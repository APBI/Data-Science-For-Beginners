<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "02ce904bc1e2bfabb7dc05c25aae375c",
  "translation_date": "2025-09-04T19:31:38+00:00",
  "source_file": "3-Data-Visualization/10-visualization-distributions/README.md",
  "language_code": "no"
}
-->
# Visualisering av fordelinger

|![ Sketchnote av [(@sketchthedocs)](https://sketchthedocs.dev) ](../../sketchnotes/10-Visualizing-Distributions.png)|
|:---:|
| Visualisering av fordelinger - _Sketchnote av [@nitya](https://twitter.com/nitya)_ |

I forrige leksjon lærte du noen interessante fakta om et datasett om fuglene i Minnesota. Du fant noen feilaktige data ved å visualisere uteliggere og så på forskjellene mellom fuglekategorier basert på deres maksimale lengde.

## [Quiz før leksjonen](https://purple-hill-04aebfb03.1.azurestaticapps.net/quiz/18)
## Utforsk fugledatasettet

En annen måte å undersøke data på er ved å se på fordelingen, eller hvordan dataene er organisert langs en akse. Kanskje du for eksempel vil lære om den generelle fordelingen, for dette datasettet, av maksimal vingespenn eller maksimal kroppsmasse for fuglene i Minnesota.

La oss oppdage noen fakta om fordelingen av data i dette datasettet. I _notebook.ipynb_-filen i roten av denne leksjonsmappen, importer Pandas, Matplotlib og dataene dine:

```python
import pandas as pd
import matplotlib.pyplot as plt
birds = pd.read_csv('../../data/birds.csv')
birds.head()
```

|      | Navn                         | VitenskapeligNavn      | Kategori              | Orden        | Familie  | Slekt       | Bevaringsstatus     | MinLengde | MaksLengde | MinKroppsmasse | MaksKroppsmasse | MinVingespenn | MaksVingespenn |
| ---: | :--------------------------- | :--------------------- | :-------------------- | :----------- | :------- | :---------- | :----------------- | --------: | --------: | ------------: | -------------: | ------------: | -------------: |
|    0 | Svartbukket plystreand       | Dendrocygna autumnalis | Ender/Gjess/Vannfugl  | Anseriformes | Anatidae | Dendrocygna | LC                 |        47 |        56 |           652 |           1020 |            76 |            94 |
|    1 | Rødbrun plystreand           | Dendrocygna bicolor    | Ender/Gjess/Vannfugl  | Anseriformes | Anatidae | Dendrocygna | LC                 |        45 |        53 |           712 |           1050 |            85 |            93 |
|    2 | Snøgås                       | Anser caerulescens     | Ender/Gjess/Vannfugl  | Anseriformes | Anatidae | Anser       | LC                 |        64 |        79 |          2050 |           4050 |           135 |           165 |
|    3 | Ross' gås                    | Anser rossii           | Ender/Gjess/Vannfugl  | Anseriformes | Anatidae | Anser       | LC                 |      57.3 |        64 |          1066 |           1567 |           113 |           116 |
|    4 | Større hvitkinngås           | Anser albifrons        | Ender/Gjess/Vannfugl  | Anseriformes | Anatidae | Anser       | LC                 |        64 |        81 |          1930 |           3310 |           130 |           165 |

Generelt kan du raskt se hvordan dataene er fordelt ved å bruke et spredningsdiagram, slik vi gjorde i forrige leksjon:

```python
birds.plot(kind='scatter',x='MaxLength',y='Order',figsize=(12,8))

plt.title('Max Length per Order')
plt.ylabel('Order')
plt.xlabel('Max Length')

plt.show()
```
![maks lengde per orden](../../../../translated_images/scatter-wb.9d98b0ed7f0388af979441853361a11df5f518f5307938a503ca7913e986111b.no.png)

Dette gir en oversikt over den generelle fordelingen av kroppslengde per fugleorden, men det er ikke den optimale måten å vise ekte fordelinger. Den oppgaven håndteres vanligvis ved å lage et histogram.

## Arbeid med histogrammer

Matplotlib tilbyr veldig gode måter å visualisere datafordeling ved hjelp av histogrammer. Denne typen diagram ligner på et stolpediagram der fordelingen kan sees via oppgang og nedgang i stolpene. For å lage et histogram trenger du numeriske data. For å lage et histogram kan du plotte et diagram og definere typen som 'hist' for histogram. Dette diagrammet viser fordelingen av MaksKroppsmasse for hele datasettets numeriske data. Ved å dele opp datasettet i mindre grupper kan det vise fordelingen av verdiene:

```python
birds['MaxBodyMass'].plot(kind = 'hist', bins = 10, figsize = (12,12))
plt.show()
```
![fordeling over hele datasettet](../../../../translated_images/dist1-wb.0d0cac82e2974fbbec635826fefead401af795f82e2279e2e2678bf2c117d827.no.png)

Som du kan se, faller de fleste av de 400+ fuglene i dette datasettet innenfor området under 2000 for deres Maks Kroppsmasse. Få mer innsikt i dataene ved å endre `bins`-parameteren til et høyere tall, for eksempel 30:

```python
birds['MaxBodyMass'].plot(kind = 'hist', bins = 30, figsize = (12,12))
plt.show()
```
![fordeling over hele datasettet med større bins-parameter](../../../../translated_images/dist2-wb.2c0a7a3499b2fbf561e9f93b69f265dfc538dc78f6de15088ba84a88152e26ba.no.png)

Dette diagrammet viser fordelingen på en litt mer detaljert måte. Et diagram som er mindre skjevt mot venstre kan opprettes ved å sørge for at du bare velger data innenfor et gitt område:

Filtrer dataene dine for å få kun de fuglene hvis kroppsmasse er under 60, og vis 40 `bins`:

```python
filteredBirds = birds[(birds['MaxBodyMass'] > 1) & (birds['MaxBodyMass'] < 60)]      
filteredBirds['MaxBodyMass'].plot(kind = 'hist',bins = 40,figsize = (12,12))
plt.show()     
```
![filtrert histogram](../../../../translated_images/dist3-wb.64b88db7f9780200bd486a2c2a3252548dd439672dbd3f778193db7f654b100c.no.png)

✅ Prøv noen andre filtre og datapunkter. For å se hele fordelingen av dataene, fjern `['MaxBodyMass']`-filteret for å vise merkede fordelinger.

Histogrammet tilbyr også noen fine farge- og merkingsforbedringer du kan prøve:

Lag et 2D-histogram for å sammenligne forholdet mellom to fordelinger. La oss sammenligne `MaxBodyMass` vs. `MaxLength`. Matplotlib tilbyr en innebygd måte å vise konvergens ved hjelp av lysere farger:

```python
x = filteredBirds['MaxBodyMass']
y = filteredBirds['MaxLength']

fig, ax = plt.subplots(tight_layout=True)
hist = ax.hist2d(x, y)
```
Det ser ut til å være en forventet korrelasjon mellom disse to elementene langs en forventet akse, med ett spesielt sterkt punkt for konvergens:

![2D-plott](../../../../translated_images/2D-wb.ae22fdd33936507a41e3af22e11e4903b04a9be973b23a4e05214efaccfd66c8.no.png)

Histogrammer fungerer godt som standard for numeriske data. Hva om du trenger å se fordelinger basert på tekstdata? 
## Utforsk datasettet for fordelinger ved hjelp av tekstdata 

Dette datasettet inneholder også god informasjon om fuglekategori og dens slekt, art og familie, samt bevaringsstatus. La oss undersøke denne bevaringsinformasjonen. Hva er fordelingen av fuglene basert på deres bevaringsstatus?

> ✅ I datasettet brukes flere akronymer for å beskrive bevaringsstatus. Disse akronymene kommer fra [IUCN Red List Categories](https://www.iucnredlist.org/), en organisasjon som katalogiserer arters status.
> 
> - CR: Kritisk truet
> - EN: Truet
> - EX: Utdødd
> - LC: Minst bekymring
> - NT: Nær truet
> - VU: Sårbar

Disse er tekstbaserte verdier, så du må gjøre en transformasjon for å lage et histogram. Bruk filteredBirds-datasettet til å vise bevaringsstatusen sammen med Minimum Vingespenn. Hva ser du? 

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

![vingespenn og bevaringsstatus](../../../../translated_images/histogram-conservation-wb.3c40450eb072c14de7a1a3ec5c0fcba4995531024760741b392911b567fd8b70.no.png)

Det ser ikke ut til å være en god korrelasjon mellom minimum vingespenn og bevaringsstatus. Test andre elementer i datasettet ved hjelp av denne metoden. Du kan også prøve forskjellige filtre. Finner du noen korrelasjon?

## Tetthetsdiagrammer

Du har kanskje lagt merke til at histogrammene vi har sett på så langt er 'trinnvise' og ikke flyter jevnt i en bue. For å vise et jevnere tetthetsdiagram kan du prøve et tetthetsplott.

For å arbeide med tetthetsdiagrammer, bli kjent med et nytt plottebibliotek, [Seaborn](https://seaborn.pydata.org/generated/seaborn.kdeplot.html). 

Last inn Seaborn og prøv et grunnleggende tetthetsdiagram:

```python
import seaborn as sns
import matplotlib.pyplot as plt
sns.kdeplot(filteredBirds['MinWingspan'])
plt.show()
```
![Tetthetsdiagram](../../../../translated_images/density1.8801043bd4af2567b0f706332b5853c7614e5e4b81b457acc27eb4e092a65cbd.no.png)

Du kan se hvordan diagrammet gjenspeiler det forrige for Minimum Vingespenn-data; det er bare litt jevnere. Ifølge Seaborns dokumentasjon, "Sammenlignet med et histogram kan KDE produsere et diagram som er mindre rotete og mer tolkbart, spesielt når man tegner flere fordelinger. Men det har potensial til å introdusere forvrengninger hvis den underliggende fordelingen er begrenset eller ikke jevn. Som et histogram avhenger kvaliteten på representasjonen også av valget av gode jevningsparametere." [kilde](https://seaborn.pydata.org/generated/seaborn.kdeplot.html) Med andre ord, uteliggere vil som alltid få diagrammene dine til å oppføre seg dårlig.

Hvis du ville gjenbesøke den hakkete MaksKroppsmasse-linjen i det andre diagrammet du laget, kunne du jevne den ut veldig godt ved å gjenskape den ved hjelp av denne metoden:

```python
sns.kdeplot(filteredBirds['MaxBodyMass'])
plt.show()
```
![jevn kroppsmasse-linje](../../../../translated_images/density2.8e7647257060ff544a1aaded57e8dd1887586bfe340139e9b77ac1e5287f7977.no.png)

Hvis du ville ha en jevn, men ikke for jevn linje, kan du redigere `bw_adjust`-parameteren: 

```python
sns.kdeplot(filteredBirds['MaxBodyMass'], bw_adjust=.2)
plt.show()
```
![mindre jevn kroppsmasse-linje](../../../../translated_images/density3.84ae27da82f31e6b83ad977646f029a1d21186574d7581facd70123b3eb257ee.no.png)

✅ Les om parameterne som er tilgjengelige for denne typen diagram og eksperimenter!

Denne typen diagram tilbyr vakre og forklarende visualiseringer. Med noen få linjer kode kan du for eksempel vise tettheten av maksimal kroppsmasse per fugleorden:

```python
sns.kdeplot(
   data=filteredBirds, x="MaxBodyMass", hue="Order",
   fill=True, common_norm=False, palette="crest",
   alpha=.5, linewidth=0,
)
```

![kroppsmasse per orden](../../../../translated_images/density4.e9d6c033f15c500fd33df94cb592b9f5cf1ed2a3d213c448a3f9e97ba39573ce.no.png)

Du kan også kartlegge tettheten av flere variabler i ett diagram. Test MaksLengde og MinLengde for en fugl sammenlignet med deres bevaringsstatus:

```python
sns.kdeplot(data=filteredBirds, x="MinLength", y="MaxLength", hue="ConservationStatus")
```

![flere tettheter, lagt oppå hverandre](../../../../translated_images/multi.56548caa9eae8d0fd9012a8586295538c7f4f426e2abc714ba070e2e4b1fc2c1.no.png)

Kanskje det er verdt å undersøke om klyngen av 'Sårbare' fugler basert på deres lengder er meningsfull eller ikke.

## 🚀 Utfordring

Histogrammer er en mer sofistikert type diagram enn grunnleggende spredningsdiagrammer, stolpediagrammer eller linjediagrammer. Gjør et søk på internett for å finne gode eksempler på bruk av histogrammer. Hvordan brukes de, hva demonstrerer de, og innen hvilke felt eller områder brukes de ofte?

## [Quiz etter leksjonen](https://ff-quizzes.netlify.app/en/ds/)

## Gjennomgang og selvstudium

I denne leksjonen brukte du Matplotlib og begynte å arbeide med Seaborn for å vise mer sofistikerte diagrammer. Gjør litt research på `kdeplot` i Seaborn, en "kontinuerlig sannsynlighetstetthetskurve i én eller flere dimensjoner". Les gjennom [dokumentasjonen](https://seaborn.pydata.org/generated/seaborn.kdeplot.html) for å forstå hvordan det fungerer.

## Oppgave

[Bruk ferdighetene dine](assignment.md)

---

**Ansvarsfraskrivelse**:  
Dette dokumentet er oversatt ved hjelp av AI-oversettelsestjenesten [Co-op Translator](https://github.com/Azure/co-op-translator). Selv om vi streber etter nøyaktighet, vær oppmerksom på at automatiserte oversettelser kan inneholde feil eller unøyaktigheter. Det originale dokumentet på sitt opprinnelige språk bør anses som den autoritative kilden. For kritisk informasjon anbefales profesjonell menneskelig oversettelse. Vi er ikke ansvarlige for misforståelser eller feiltolkninger som oppstår ved bruk av denne oversettelsen.