<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "0764fd4077f3f04a1d968ec371227744",
  "translation_date": "2025-09-06T11:48:36+00:00",
  "source_file": "3-Data-Visualization/12-visualization-relationships/README.md",
  "language_code": "hr"
}
-->
# Vizualizacija odnosa: Sve o medu 🍯

|![ Sketchnote by [(@sketchthedocs)](https://sketchthedocs.dev) ](../../sketchnotes/12-Visualizing-Relationships.png)|
|:---:|
|Vizualizacija odnosa - _Sketchnote by [@nitya](https://twitter.com/nitya)_ |

Nastavljajući s prirodnim fokusom našeg istraživanja, istražimo zanimljive vizualizacije koje prikazuju odnose između različitih vrsta meda, prema skupu podataka dobivenom od [Ministarstva poljoprivrede Sjedinjenih Država](https://www.nass.usda.gov/About_NASS/index.php).

Ovaj skup podataka sadrži oko 600 stavki i prikazuje proizvodnju meda u mnogim američkim saveznim državama. Na primjer, možete pogledati broj kolonija, prinos po koloniji, ukupnu proizvodnju, zalihe, cijenu po funti i vrijednost proizvedenog meda u određenoj državi od 1998. do 2012., s jednim redom po godini za svaku državu.

Bilo bi zanimljivo vizualizirati odnos između proizvodnje određene države po godini i, na primjer, cijene meda u toj državi. Alternativno, mogli biste vizualizirati odnos između prinosa meda po koloniji u različitim državama. Ovo vremensko razdoblje obuhvaća razorni fenomen 'CCD' ili 'Sindrom kolapsa kolonija', prvi put zabilježen 2006. godine (http://npic.orst.edu/envir/ccd.html), što čini ovaj skup podataka posebno značajnim za proučavanje. 🐝

## [Kviz prije predavanja](https://ff-quizzes.netlify.app/en/ds/quiz/22)

U ovoj lekciji možete koristiti Seaborn, biblioteku koju ste već koristili, kao odličan alat za vizualizaciju odnosa između varijabli. Posebno je zanimljiva funkcija `relplot` u Seabornu, koja omogućuje scatter plotove i linijske grafove za brzu vizualizaciju '[statističkih odnosa](https://seaborn.pydata.org/tutorial/relational.html?highlight=relationships)', što pomaže znanstvenicima u podacima da bolje razumiju kako su varijable međusobno povezane.

## Scatterplotovi

Koristite scatterplot za prikaz kako se cijena meda razvijala iz godine u godinu, po državama. Seaborn, koristeći `relplot`, praktično grupira podatke po državama i prikazuje točke za kategorijske i numeričke podatke.

Započnimo uvozom podataka i biblioteke Seaborn:

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
honey = pd.read_csv('../../data/honey.csv')
honey.head()
```
Primijetit ćete da podaci o medu sadrže nekoliko zanimljivih stupaca, uključujući godinu i cijenu po funti. Istražimo ove podatke grupirane po američkim državama:

| država | brojkol | prinospokol | ukupnaprod | zalihe   | cijenapofunti | vrijednostprod | godina |
| ------ | ------- | ----------- | ---------- | -------- | ------------- | -------------- | ------ |
| AL     | 16000   | 71          | 1136000    | 159000   | 0.72          | 818000         | 1998   |
| AZ     | 55000   | 60          | 3300000    | 1485000  | 0.64          | 2112000        | 1998   |
| AR     | 53000   | 65          | 3445000    | 1688000  | 0.59          | 2033000        | 1998   |
| CA     | 450000  | 83          | 37350000   | 12326000 | 0.62          | 23157000       | 1998   |
| CO     | 27000   | 72          | 1944000    | 1594000  | 0.7           | 1361000        | 1998   |

Napravite osnovni scatterplot za prikaz odnosa između cijene po funti meda i države podrijetla. Postavite `y` os dovoljno visoko da prikaže sve države:

```python
sns.relplot(x="priceperlb", y="state", data=honey, height=15, aspect=.5);
```
![scatterplot 1](../../../../translated_images/scatter1.5e1aa5fd6706c5d12b5e503ccb77f8a930f8620f539f524ddf56a16c039a5d2f.hr.png)

Sada prikažite iste podatke s paletom boja inspiriranom medom kako biste pokazali kako se cijena mijenja tijekom godina. To možete učiniti dodavanjem parametra 'hue' za prikaz promjena iz godine u godinu:

> ✅ Saznajte više o [paletama boja koje možete koristiti u Seabornu](https://seaborn.pydata.org/tutorial/color_palettes.html) - isprobajte prekrasnu paletu boja poput duge!

```python
sns.relplot(x="priceperlb", y="state", hue="year", palette="YlOrBr", data=honey, height=15, aspect=.5);
```
![scatterplot 2](../../../../translated_images/scatter2.c0041a58621ca702990b001aa0b20cd68c1e1814417139af8a7211a2bed51c5f.hr.png)

S ovom promjenom palete boja možete jasno vidjeti snažan napredak tijekom godina u pogledu cijene meda po funti. Ako pogledate uzorak podataka za provjeru (na primjer, odaberite državu Arizonu), možete uočiti obrazac povećanja cijene iz godine u godinu, uz nekoliko iznimaka:

| država | brojkol | prinospokol | ukupnaprod | zalihe  | cijenapofunti | vrijednostprod | godina |
| ------ | ------- | ----------- | ---------- | ------- | ------------- | -------------- | ------ |
| AZ     | 55000   | 60          | 3300000    | 1485000 | 0.64          | 2112000        | 1998   |
| AZ     | 52000   | 62          | 3224000    | 1548000 | 0.62          | 1999000        | 1999   |
| AZ     | 40000   | 59          | 2360000    | 1322000 | 0.73          | 1723000        | 2000   |
| AZ     | 43000   | 59          | 2537000    | 1142000 | 0.72          | 1827000        | 2001   |
| AZ     | 38000   | 63          | 2394000    | 1197000 | 1.08          | 2586000        | 2002   |
| AZ     | 35000   | 72          | 2520000    | 983000  | 1.34          | 3377000        | 2003   |
| AZ     | 32000   | 55          | 1760000    | 774000  | 1.11          | 1954000        | 2004   |
| AZ     | 36000   | 50          | 1800000    | 720000  | 1.04          | 1872000        | 2005   |
| AZ     | 30000   | 65          | 1950000    | 839000  | 0.91          | 1775000        | 2006   |
| AZ     | 30000   | 64          | 1920000    | 902000  | 1.26          | 2419000        | 2007   |
| AZ     | 25000   | 64          | 1600000    | 336000  | 1.26          | 2016000        | 2008   |
| AZ     | 20000   | 52          | 1040000    | 562000  | 1.45          | 1508000        | 2009   |
| AZ     | 24000   | 77          | 1848000    | 665000  | 1.52          | 2809000        | 2010   |
| AZ     | 23000   | 53          | 1219000    | 427000  | 1.55          | 1889000        | 2011   |
| AZ     | 22000   | 46          | 1012000    | 253000  | 1.79          | 1811000        | 2012   |

Drugi način za vizualizaciju ovog napretka je korištenje veličine umjesto boje. Za korisnike s poteškoćama u razlikovanju boja, ovo bi mogla biti bolja opcija. Uredite svoju vizualizaciju tako da povećanje cijene prikažete povećanjem opsega točaka:

```python
sns.relplot(x="priceperlb", y="state", size="year", data=honey, height=15, aspect=.5);
```
Možete vidjeti kako se veličina točaka postupno povećava.

![scatterplot 3](../../../../translated_images/scatter3.3c160a3d1dcb36b37900ebb4cf97f34036f28ae2b7b8e6062766c7c1dfc00853.hr.png)

Je li ovo jednostavan slučaj ponude i potražnje? Zbog čimbenika poput klimatskih promjena i kolapsa kolonija, je li dostupno manje meda za kupnju iz godine u godinu, pa cijena raste?

Kako bismo otkrili korelaciju između nekih varijabli u ovom skupu podataka, istražimo nekoliko linijskih grafova.

## Linijski grafovi

Pitanje: Postoji li jasan porast cijene meda po funti iz godine u godinu? To možete najlakše otkriti stvaranjem jednostavnog linijskog grafa:

```python
sns.relplot(x="year", y="priceperlb", kind="line", data=honey);
```
Odgovor: Da, uz nekoliko iznimaka oko 2003. godine:

![line chart 1](../../../../translated_images/line1.f36eb465229a3b1fe385cdc93861aab3939de987d504b05de0b6cd567ef79f43.hr.png)

✅ Budući da Seaborn agregira podatke u jednu liniju, prikazuje "više mjerenja za svaku vrijednost x tako što crta srednju vrijednost i interval pouzdanosti od 95% oko srednje vrijednosti". [Izvor](https://seaborn.pydata.org/tutorial/relational.html). Ovo ponašanje koje oduzima vrijeme može se onemogućiti dodavanjem `ci=None`.

Pitanje: Pa, možemo li također vidjeti porast u opskrbi medom oko 2003. godine? Što ako pogledate ukupnu proizvodnju iz godine u godinu?

```python
sns.relplot(x="year", y="totalprod", kind="line", data=honey);
```

![line chart 2](../../../../translated_images/line2.a5b3493dc01058af6402e657aaa9ae1125fafb5e7d6630c777aa60f900a544e4.hr.png)

Odgovor: Ne baš. Ako pogledate ukupnu proizvodnju, čini se da je zapravo porasla te godine, iako općenito količina proizvedenog meda opada tijekom tih godina.

Pitanje: U tom slučaju, što je moglo uzrokovati taj skok u cijeni meda oko 2003. godine?

Kako bismo to otkrili, možemo istražiti facet grid.

## Facet gridovi

Facet gridovi uzimaju jedan aspekt vašeg skupa podataka (u našem slučaju, možete odabrati 'godinu' kako biste izbjegli previše proizvedenih gridova). Seaborn tada može napraviti graf za svaki od tih aspekata vaših odabranih x i y koordinata za lakšu vizualnu usporedbu. Ističe li se 2003. godina u ovoj vrsti usporedbe?

Napravite facet grid koristeći `relplot`, kako preporučuje [dokumentacija za Seaborn](https://seaborn.pydata.org/generated/seaborn.FacetGrid.html?highlight=facetgrid#seaborn.FacetGrid).

```python
sns.relplot(
    data=honey, 
    x="yieldpercol", y="numcol",
    col="year", 
    col_wrap=3,
    kind="line"
    )
```
U ovoj vizualizaciji možete usporediti prinos po koloniji i broj kolonija iz godine u godinu, usporedno s postavkom wrap na 3 za stupce:

![facet grid](../../../../translated_images/facet.6a34851dcd540050dcc0ead741be35075d776741668dd0e42f482c89b114c217.hr.png)

Za ovaj skup podataka, ništa posebno ne iskače u vezi s brojem kolonija i njihovim prinosom, iz godine u godinu i iz države u državu. Postoji li drugačiji način za pronalaženje korelacije između ove dvije varijable?

## Dvostruki linijski grafovi

Isprobajte višelinijski graf superponiranjem dvaju linijskih grafova jedan na drugi, koristeći Seabornov 'despine' za uklanjanje gornjih i desnih osi, te koristeći `ax.twinx` [iz Matplotliba](https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.twinx.html). Twinx omogućuje dijagramu dijeljenje x osi i prikaz dviju y osi. Dakle, prikažite prinos po koloniji i broj kolonija, superponirano:

```python
fig, ax = plt.subplots(figsize=(12,6))
lineplot = sns.lineplot(x=honey['year'], y=honey['numcol'], data=honey, 
                        label = 'Number of bee colonies', legend=False)
sns.despine()
plt.ylabel('# colonies')
plt.title('Honey Production Year over Year');

ax2 = ax.twinx()
lineplot2 = sns.lineplot(x=honey['year'], y=honey['yieldpercol'], ax=ax2, color="r", 
                         label ='Yield per colony', legend=False) 
sns.despine(right=False)
plt.ylabel('colony yield')
ax.figure.legend();
```
![superimposed plots](../../../../translated_images/dual-line.a4c28ce659603fab2c003f4df816733df2bf41d1facb7de27989ec9afbf01b33.hr.png)

Iako ništa posebno ne iskače oko 2003. godine, ovo nam omogućuje da završimo lekciju na malo sretnijoj noti: iako općenito dolazi do smanjenja broja kolonija, broj kolonija se stabilizira čak i ako njihov prinos po koloniji opada.

Naprijed, pčele! 🐝❤️

## 🚀 Izazov

U ovoj lekciji naučili ste nešto više o drugim načinima korištenja scatterplotova i linijskih gridova, uključujući facet gridove. Izazovite se da napravite facet grid koristeći neki drugi skup podataka, možda onaj koji ste koristili prije ovih lekcija. Obratite pažnju na to koliko dugo traje njihovo stvaranje i koliko pažljivo trebate biti s brojem gridova koje trebate nacrtati koristeći ove tehnike.

## [Kviz nakon predavanja](https://ff-quizzes.netlify.app/en/ds/quiz/23)

## Pregled i samostalno učenje

Linijski grafovi mogu biti jednostavni ili prilično složeni. Pročitajte malo više u [dokumentaciji za Seaborn](https://seaborn.pydata.org/generated/seaborn.lineplot.html) o raznim načinima na koje ih možete izgraditi. Pokušajte unaprijediti linijske grafove koje ste izradili u ovoj lekciji koristeći druge metode navedene u dokumentaciji.

## Zadatak

[Zaronite u košnicu](assignment.md)

---

**Odricanje od odgovornosti**:  
Ovaj dokument je preveden korištenjem AI usluge za prevođenje [Co-op Translator](https://github.com/Azure/co-op-translator). Iako nastojimo osigurati točnost, imajte na umu da automatski prijevodi mogu sadržavati pogreške ili netočnosti. Izvorni dokument na izvornom jeziku treba smatrati mjerodavnim izvorom. Za ključne informacije preporučuje se profesionalni prijevod od strane stručnjaka. Ne preuzimamo odgovornost za bilo kakva nesporazuma ili pogrešna tumačenja koja mogu proizaći iz korištenja ovog prijevoda.