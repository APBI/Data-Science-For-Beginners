<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "02ce904bc1e2bfabb7dc05c25aae375c",
  "translation_date": "2025-09-04T22:02:20+00:00",
  "source_file": "3-Data-Visualization/10-visualization-distributions/README.md",
  "language_code": "hr"
}
-->
# Vizualizacija distribucija

|![ Sketchnote autor [(@sketchthedocs)](https://sketchthedocs.dev) ](../../sketchnotes/10-Visualizing-Distributions.png)|
|:---:|
| Vizualizacija distribucija - _Sketchnote autor [@nitya](https://twitter.com/nitya)_ |

U prethodnoj lekciji naučili ste neke zanimljive činjenice o skupu podataka o pticama Minnesote. Pronašli ste pogrešne podatke vizualizacijom odstupanja i pogledali razlike između kategorija ptica prema njihovoj maksimalnoj duljini.

## [Kviz prije predavanja](https://purple-hill-04aebfb03.1.azurestaticapps.net/quiz/18)
## Istražite skup podataka o pticama

Još jedan način za istraživanje podataka je promatranje njihove distribucije, odnosno kako su podaci organizirani duž osi. Možda, na primjer, želite saznati opću distribuciju maksimalnog raspona krila ili maksimalne tjelesne mase ptica Minnesote u ovom skupu podataka.

Otkrijmo neke činjenice o distribucijama podataka u ovom skupu podataka. U datoteci _notebook.ipynb_ u korijenskoj mapi ove lekcije, uvezite Pandas, Matplotlib i svoje podatke:

```python
import pandas as pd
import matplotlib.pyplot as plt
birds = pd.read_csv('../../data/birds.csv')
birds.head()
```

|      | Ime                          | ZnanstvenoIme          | Kategorija            | Red          | Porodica | Rod         | StatusOčuvanja     | MinDuljina | MaxDuljina | MinTjelesnaMasa | MaxTjelesnaMasa | MinRasponKrila | MaxRasponKrila |
| ---: | :--------------------------- | :--------------------- | :-------------------- | :----------- | :------- | :---------- | :----------------- | ----------: | ----------: | --------------: | --------------: | --------------: | --------------: |
|    0 | Crnoprsi zviždukavi patak    | Dendrocygna autumnalis | Patke/Guske/Vodene ptice | Anseriformes | Anatidae | Dendrocygna | LC                 |        47   |        56   |           652   |          1020   |            76   |            94   |
|    1 | Riđi zviždukavi patak        | Dendrocygna bicolor    | Patke/Guske/Vodene ptice | Anseriformes | Anatidae | Dendrocygna | LC                 |        45   |        53   |           712   |          1050   |            85   |            93   |
|    2 | Snježna guska                | Anser caerulescens     | Patke/Guske/Vodene ptice | Anseriformes | Anatidae | Anser       | LC                 |        64   |        79   |          2050   |          4050   |           135   |           165   |
|    3 | Rossova guska                | Anser rossii           | Patke/Guske/Vodene ptice | Anseriformes | Anatidae | Anser       | LC                 |      57.3   |        64   |          1066   |          1567   |           113   |           116   |
|    4 | Velika bijeloprsa guska      | Anser albifrons        | Patke/Guske/Vodene ptice | Anseriformes | Anatidae | Anser       | LC                 |        64   |        81   |          1930   |          3310   |           130   |           165   |

Općenito, distribuciju podataka možete brzo pregledati pomoću raspršenog dijagrama, kao što smo to učinili u prethodnoj lekciji:

```python
birds.plot(kind='scatter',x='MaxLength',y='Order',figsize=(12,8))

plt.title('Max Length per Order')
plt.ylabel('Order')
plt.xlabel('Max Length')

plt.show()
```
![maksimalna duljina po redu](../../../../3-Data-Visualization/10-visualization-distributions/images/scatter-wb.png)

Ovo daje pregled opće distribucije duljine tijela po redu ptica, ali nije optimalan način za prikaz stvarnih distribucija. Taj zadatak obično se rješava stvaranjem histograma.

## Rad s histogramima

Matplotlib nudi vrlo dobre načine za vizualizaciju distribucije podataka pomoću histograma. Ova vrsta grafikona slična je stupčastom grafikonu gdje se distribucija može vidjeti kroz porast i pad stupaca. Za izradu histograma potrebni su vam numerički podaci. Za izradu histograma možete nacrtati grafikon definirajući vrstu kao 'hist' za histogram. Ovaj grafikon prikazuje distribuciju MaxBodyMass za cijeli raspon numeričkih podataka u skupu podataka. Dijeljenjem niza podataka u manje segmente (bins), može prikazati distribuciju vrijednosti podataka:

```python
birds['MaxBodyMass'].plot(kind = 'hist', bins = 10, figsize = (12,12))
plt.show()
```
![distribucija za cijeli skup podataka](../../../../3-Data-Visualization/10-visualization-distributions/images/dist1-wb.png)

Kao što vidite, većina od 400+ ptica u ovom skupu podataka spada u raspon ispod 2000 za njihovu maksimalnu tjelesnu masu. Dobijte više uvida u podatke promjenom parametra `bins` na veći broj, poput 30:

```python
birds['MaxBodyMass'].plot(kind = 'hist', bins = 30, figsize = (12,12))
plt.show()
```
![distribucija za cijeli skup podataka s većim bins parametrom](../../../../3-Data-Visualization/10-visualization-distributions/images/dist2-wb.png)

Ovaj grafikon prikazuje distribuciju na malo detaljniji način. Grafikon manje nagnut ulijevo mogao bi se stvoriti osiguravanjem da odaberete samo podatke unutar određenog raspona:

Filtrirajte svoje podatke kako biste dobili samo one ptice čija je tjelesna masa ispod 60 i prikažite 40 `bins`:

```python
filteredBirds = birds[(birds['MaxBodyMass'] > 1) & (birds['MaxBodyMass'] < 60)]      
filteredBirds['MaxBodyMass'].plot(kind = 'hist',bins = 40,figsize = (12,12))
plt.show()     
```
![filtrirani histogram](../../../../3-Data-Visualization/10-visualization-distributions/images/dist3-wb.png)

✅ Isprobajte neke druge filtre i podatkovne točke. Da biste vidjeli punu distribuciju podataka, uklonite filter `['MaxBodyMass']` kako biste prikazali označene distribucije.

Histogram također nudi neke lijepe mogućnosti za boje i označavanje koje možete isprobati:

Napravite 2D histogram za usporedbu odnosa između dvije distribucije. Usporedimo `MaxBodyMass` i `MaxLength`. Matplotlib nudi ugrađeni način za prikaz konvergencije pomoću svjetlijih boja:

```python
x = filteredBirds['MaxBodyMass']
y = filteredBirds['MaxLength']

fig, ax = plt.subplots(tight_layout=True)
hist = ax.hist2d(x, y)
```
Čini se da postoji očekivana korelacija između ova dva elementa duž očekivane osi, s jednom posebno jakom točkom konvergencije:

![2D grafikon](../../../../3-Data-Visualization/10-visualization-distributions/images/2D-wb.png)

Histogrami dobro funkcioniraju za numeričke podatke. Što ako trebate vidjeti distribucije prema tekstualnim podacima? 

## Istražite skup podataka za distribucije koristeći tekstualne podatke 

Ovaj skup podataka također uključuje korisne informacije o kategoriji ptica, njihovom rodu, vrsti i porodici, kao i o njihovom statusu očuvanja. Istražimo ove informacije o očuvanju. Kakva je distribucija ptica prema njihovom statusu očuvanja?

> ✅ U skupu podataka koristi se nekoliko akronima za opis statusa očuvanja. Ovi akronimi dolaze iz [IUCN-ovih kategorija Crvene liste](https://www.iucnredlist.org/), organizacije koja katalogizira status vrsta.
> 
> - CR: Kritično ugrožena
> - EN: Ugrožena
> - EX: Izumrla
> - LC: Najmanje zabrinjavajuća
> - NT: Blizu ugroženosti
> - VU: Ranjiva

Ovo su tekstualne vrijednosti, pa ćete morati napraviti transformaciju kako biste stvorili histogram. Koristeći filtriraniBirds dataframe, prikažite njegov status očuvanja uz minimalni raspon krila. Što primjećujete?

```python
x1 = filteredBirds.loc[filteredBirds.ConservationStatus=='EX', 'MinWingspan']
x2 = filteredBirds.loc[filteredBirds.ConservationStatus=='CR', 'MinWingspan']
x3 = filteredBirds.loc[filteredBirds.ConservationStatus=='EN', 'MinWingspan']
x4 = filteredBirds.loc[filteredBirds.ConservationStatus=='NT', 'MinWingspan']
x5 = filteredBirds.loc[filteredBirds.ConservationStatus=='VU', 'MinWingspan']
x6 = filteredBirds.loc[filteredBirds.ConservationStatus=='LC', 'MinWingspan']

kwargs = dict(alpha=0.5, bins=20)

plt.hist(x1, **kwargs, color='red', label='Extinct')
plt.hist(x2, **kwargs, color='orange', label='Critically Endangered')
plt.hist(x3, **kwargs, color='yellow', label='Endangered')
plt.hist(x4, **kwargs, color='green', label='Near Threatened')
plt.hist(x5, **kwargs, color='blue', label='Vulnerable')
plt.hist(x6, **kwargs, color='gray', label='Least Concern')

plt.gca().set(title='Conservation Status', ylabel='Min Wingspan')
plt.legend();
```

![raspon krila i status očuvanja](../../../../3-Data-Visualization/10-visualization-distributions/images/histogram-conservation-wb.png)

Ne čini se da postoji dobra korelacija između minimalnog raspona krila i statusa očuvanja. Testirajte druge elemente skupa podataka koristeći ovu metodu. Možete isprobati i različite filtre. Nalazite li neku korelaciju?

## Grafovi gustoće

Možda ste primijetili da histogrami koje smo do sada gledali imaju 'stepenasti' izgled i ne teku glatko u luku. Za prikaz glatkijeg grafikona gustoće možete isprobati graf gustoće.

Za rad s grafovima gustoće upoznajte se s novom bibliotekom za crtanje, [Seaborn](https://seaborn.pydata.org/generated/seaborn.kdeplot.html). 

Učitajte Seaborn i isprobajte osnovni graf gustoće:

```python
import seaborn as sns
import matplotlib.pyplot as plt
sns.kdeplot(filteredBirds['MinWingspan'])
plt.show()
```
![Graf gustoće](../../../../3-Data-Visualization/10-visualization-distributions/images/density1.png)

Možete vidjeti kako grafikon odražava prethodni za podatke o minimalnom rasponu krila; samo je malo glađi. Prema dokumentaciji Seaborna, "U usporedbi s histogramom, KDE može proizvesti grafikon koji je manje zagušen i lakše razumljiv, posebno kada se crtaju višestruke distribucije. No, ima potencijal za uvođenje iskrivljenja ako je osnovna distribucija ograničena ili nije glatka. Kao i kod histograma, kvaliteta prikaza također ovisi o odabiru dobrih parametara zaglađivanja." [izvor](https://seaborn.pydata.org/generated/seaborn.kdeplot.html) Drugim riječima, odstupanja će, kao i uvijek, loše utjecati na vaše grafikone.

Ako želite ponovno pogledati onu nazubljenu liniju MaxBodyMass iz drugog grafikona koji ste izradili, mogli biste je vrlo dobro zagladiti ponovnim stvaranjem koristeći ovu metodu:

```python
sns.kdeplot(filteredBirds['MaxBodyMass'])
plt.show()
```
![zaglađena linija tjelesne mase](../../../../3-Data-Visualization/10-visualization-distributions/images/density2.png)

Ako želite glatku, ali ne previše glatku liniju, uredite parametar `bw_adjust`: 

```python
sns.kdeplot(filteredBirds['MaxBodyMass'], bw_adjust=.2)
plt.show()
```
![manje glatka linija tjelesne mase](../../../../3-Data-Visualization/10-visualization-distributions/images/density3.png)

✅ Pročitajte o dostupnim parametrima za ovu vrstu grafikona i eksperimentirajte!

Ova vrsta grafikona nudi prekrasno objašnjavajuće vizualizacije. S nekoliko linija koda, na primjer, možete prikazati gustoću maksimalne tjelesne mase po redu ptica:

```python
sns.kdeplot(
   data=filteredBirds, x="MaxBodyMass", hue="Order",
   fill=True, common_norm=False, palette="crest",
   alpha=.5, linewidth=0,
)
```

![tjelesna masa po redu](../../../../3-Data-Visualization/10-visualization-distributions/images/density4.png)

Također možete mapirati gustoću nekoliko varijabli na jednom grafikonu. Testirajte MaxLength i MinLength ptice u usporedbi s njihovim statusom očuvanja:

```python
sns.kdeplot(data=filteredBirds, x="MinLength", y="MaxLength", hue="ConservationStatus")
```

![višestruke gustoće, preklopljene](../../../../3-Data-Visualization/10-visualization-distributions/images/multi.png)

Možda vrijedi istražiti je li klaster 'ranjivih' ptica prema njihovim duljinama značajan ili ne.

## 🚀 Izazov

Histogrami su sofisticiranija vrsta grafikona od osnovnih raspršenih dijagrama, stupčastih grafikona ili linijskih grafikona. Potražite na internetu dobre primjere korištenja histograma. Kako se koriste, što pokazuju i u kojim se područjima ili poljima istraživanja obično koriste?

## [Kviz nakon predavanja](https://ff-quizzes.netlify.app/en/ds/)

## Pregled i samostalno učenje

U ovoj lekciji koristili ste Matplotlib i počeli raditi sa Seabornom kako biste prikazali sofisticiranije grafikone. Istražite `kdeplot` u Seabornu, "kontinuiranu krivulju gustoće vjerojatnosti u jednoj ili više dimenzija". Pročitajte [dokumentaciju](https://seaborn.pydata.org/generated/seaborn.kdeplot.html) kako biste razumjeli kako funkcionira.

## Zadatak

[Primijenite svoje vještine](assignment.md)

---

**Odricanje od odgovornosti**:  
Ovaj dokument je preveden pomoću AI usluge za prevođenje [Co-op Translator](https://github.com/Azure/co-op-translator). Iako nastojimo osigurati točnost, imajte na umu da automatski prijevodi mogu sadržavati pogreške ili netočnosti. Izvorni dokument na izvornom jeziku treba smatrati mjerodavnim izvorom. Za ključne informacije preporučuje se profesionalni prijevod od strane stručnjaka. Ne preuzimamo odgovornost za bilo kakve nesporazume ili pogrešne interpretacije proizašle iz korištenja ovog prijevoda.