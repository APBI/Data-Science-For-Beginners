<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "39f3b3a9d873eaa522c2e792ce0ca503",
  "translation_date": "2025-09-05T05:53:41+00:00",
  "source_file": "5-Data-Science-In-Cloud/18-Low-Code/README.md",
  "language_code": "sl"
}
-->
# Podatkovna znanost v oblaku: "Low code/No code" pristop

|![ Sketchnote by [(@sketchthedocs)](https://sketchthedocs.dev) ](../../sketchnotes/18-DataScience-Cloud.png)|
|:---:|
| Podatkovna znanost v oblaku: Low Code - _Sketchnote by [@nitya](https://twitter.com/nitya)_ |

Kazalo:

- [Podatkovna znanost v oblaku: "Low code/No code" pristop](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  - [Pred-predavanje kviz](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  - [1. Uvod](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [1.1 Kaj je Azure Machine Learning?](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [1.2 Projekt napovedovanja srčnega popuščanja:](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [1.3 Podatkovni niz srčnega popuščanja:](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  - [2. Low code/No code usposabljanje modela v Azure ML Studio](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [2.1 Ustvarjanje delovnega prostora Azure ML](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [2.2 Računalniški viri](../../../../5-Data-Science-In-Cloud/18-Low-Code)
      - [2.2.1 Izbira pravih možnosti za vaše računalniške vire](../../../../5-Data-Science-In-Cloud/18-Low-Code)
      - [2.2.2 Ustvarjanje računalniškega grozda](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [2.3 Nalaganje podatkovnega niza](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [2.4 Low code/No Code usposabljanje z AutoML](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  - [3. Low code/No Code uvajanje modela in uporaba končne točke](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [3.1 Uvajanje modela](../../../../5-Data-Science-In-Cloud/18-Low-Code)
    - [3.2 Uporaba končne točke](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  - [🚀 Izziv](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  - [Kviz po predavanju](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  - [Pregled in samostojno učenje](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  - [Naloga](../../../../5-Data-Science-In-Cloud/18-Low-Code)
  
## [Pred-predavanje kviz](https://ff-quizzes.netlify.app/en/ds/)

## 1. Uvod
### 1.1 Kaj je Azure Machine Learning?

Azure oblačna platforma vključuje več kot 200 izdelkov in storitev v oblaku, zasnovanih za pomoč pri ustvarjanju novih rešitev. Podatkovni znanstveniki porabijo veliko časa za raziskovanje in predobdelavo podatkov ter preizkušanje različnih algoritmov za usposabljanje modelov, da bi ustvarili natančne modele. Te naloge so časovno zahtevne in pogosto neučinkovito izkoriščajo drage računalniške vire.

[Azure ML](https://docs.microsoft.com/azure/machine-learning/overview-what-is-azure-machine-learning?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) je platforma v oblaku za gradnjo in upravljanje rešitev strojnega učenja v Azure. Ponuja širok nabor funkcij in zmogljivosti, ki pomagajo podatkovnim znanstvenikom pri pripravi podatkov, usposabljanju modelov, objavljanju napovednih storitev in spremljanju njihove uporabe. Najpomembneje je, da povečuje njihovo učinkovitost z avtomatizacijo številnih časovno zahtevnih nalog, povezanih z usposabljanjem modelov, ter omogoča uporabo računalniških virov v oblaku, ki se učinkovito prilagajajo za obdelavo velikih količin podatkov, pri čemer nastanejo stroški le ob dejanski uporabi.

Azure ML ponuja vsa orodja, ki jih razvijalci in podatkovni znanstveniki potrebujejo za svoje delovne procese strojnega učenja. Ta vključujejo:

- **Azure Machine Learning Studio**: spletni portal v Azure Machine Learning za možnosti usposabljanja modelov, uvajanja, avtomatizacije, sledenja in upravljanja sredstev z malo ali brez kode. Studio se integrira z Azure Machine Learning SDK za brezhibno izkušnjo.
- **Jupyter Notebooks**: hitro prototipiranje in testiranje modelov strojnega učenja.
- **Azure Machine Learning Designer**: omogoča gradnjo eksperimentov z modulom povleci in spusti ter uvajanje cevovodov v okolju z malo kode.
- **Avtomatizirano strojno učenje (AutoML)**: avtomatizira iterativne naloge razvoja modelov strojnega učenja, kar omogoča gradnjo modelov z visoko učinkovitostjo in produktivnostjo, ob ohranjanju kakovosti modela.
- **Označevanje podatkov**: orodje za pomoč pri strojnem učenju za samodejno označevanje podatkov.
- **Razširitev strojnega učenja za Visual Studio Code**: ponuja popolno razvojno okolje za gradnjo in upravljanje projektov strojnega učenja.
- **CLI za strojno učenje**: omogoča ukaze za upravljanje virov Azure ML iz ukazne vrstice.
- **Integracija z odprtokodnimi ogrodji**, kot so PyTorch, TensorFlow, Scikit-learn in mnogi drugi, za usposabljanje, uvajanje in upravljanje celotnega procesa strojnega učenja.
- **MLflow**: odprtokodna knjižnica za upravljanje življenjskega cikla vaših eksperimentov strojnega učenja. **MLFlow Tracking** je komponenta MLflow, ki beleži in sledi metrikam usposabljanja ter artefaktom modela, ne glede na okolje vašega eksperimenta.

### 1.2 Projekt napovedovanja srčnega popuščanja:

Ni dvoma, da je izdelava projektov najboljši način za preizkus vaših veščin in znanja. V tej lekciji bomo raziskali dva različna načina gradnje projekta podatkovne znanosti za napovedovanje srčnih napadov v Azure ML Studio, in sicer prek Low code/No code ter prek Azure ML SDK, kot je prikazano v naslednji shemi:

![project-schema](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/project-schema.PNG)

Vsak način ima svoje prednosti in slabosti. Low code/No code pristop je lažji za začetek, saj vključuje interakcijo z grafičnim uporabniškim vmesnikom (GUI), brez predhodnega znanja o kodiranju. Ta metoda omogoča hitro testiranje izvedljivosti projekta in ustvarjanje POC (Proof Of Concept). Vendar pa, ko projekt raste in je treba stvari pripraviti za produkcijo, ni izvedljivo ustvarjati virov prek GUI. Potrebno je programatično avtomatizirati vse, od ustvarjanja virov do uvajanja modela. Tukaj postane ključno znanje uporabe Azure ML SDK.

|                   | Low code/No code | Azure ML SDK              |
|-------------------|------------------|---------------------------|
| Znanje kodiranja  | Ni potrebno      | Potrebno                  |
| Čas razvoja       | Hitro in enostavno | Odvisno od znanja kodiranja |
| Pripravljeno za produkcijo | Ne               | Da                       |

### 1.3 Podatkovni niz srčnega popuščanja: 

Kardiovaskularne bolezni (CVD) so glavni vzrok smrti po vsem svetu, saj predstavljajo 31 % vseh smrti. Okoljski in vedenjski dejavniki tveganja, kot so uporaba tobaka, nezdrava prehrana in debelost, telesna neaktivnost ter škodljiva uporaba alkohola, bi lahko služili kot značilnosti za modele ocenjevanja. Sposobnost ocenjevanja verjetnosti razvoja CVD bi bila zelo koristna za preprečevanje napadov pri ljudeh z visokim tveganjem.

Kaggle je objavil [podatkovni niz srčnega popuščanja](https://www.kaggle.com/andrewmvd/heart-failure-clinical-data), ki ga bomo uporabili za ta projekt. Podatkovni niz lahko prenesete zdaj. Gre za tabelarni podatkovni niz s 13 stolpci (12 značilnosti in 1 ciljno spremenljivko) ter 299 vrsticami. 

|    | Ime spremenljivke         | Tip             | Opis                                                     | Primer            |
|----|---------------------------|-----------------|----------------------------------------------------------|-------------------|
| 1  | age                       | numerični       | starost pacienta                                         | 25                |
| 2  | anaemia                   | logični         | Zmanjšanje rdečih krvnih celic ali hemoglobina           | 0 ali 1           |
| 3  | creatinine_phosphokinase  | numerični       | Raven encima CPK v krvi                                  | 542               |
| 4  | diabetes                  | logični         | Ali ima pacient sladkorno bolezen                        | 0 ali 1           |
| 5  | ejection_fraction         | numerični       | Odstotek krvi, ki zapusti srce ob vsakem krčenju         | 45                |
| 6  | high_blood_pressure       | logični         | Ali ima pacient hipertenzijo                             | 0 ali 1           |
| 7  | platelets                 | numerični       | Trombociti v krvi                                        | 149000            |
| 8  | serum_creatinine          | numerični       | Raven serumske kreatinina v krvi                         | 0.5               |
| 9  | serum_sodium              | numerični       | Raven serumske natrija v krvi                            | jun               |
| 10 | sex                       | logični         | ženska ali moški                                         | 0 ali 1           |
| 11 | smoking                   | logični         | Ali pacient kadi                                         | 0 ali 1           |
| 12 | time                      | numerični       | obdobje spremljanja (dni)                                | 4                 |
|----|---------------------------|-----------------|----------------------------------------------------------|-------------------|
| 21 | DEATH_EVENT [Cilj]        | logični         | Ali pacient umre med obdobjem spremljanja                | 0 ali 1           |

Ko imate podatkovni niz, lahko začnemo projekt v Azure.

## 2. Low code/No code usposabljanje modela v Azure ML Studio
### 2.1 Ustvarjanje delovnega prostora Azure ML
Za usposabljanje modela v Azure ML morate najprej ustvariti delovni prostor Azure ML. Delovni prostor je najvišji vir za Azure Machine Learning, ki zagotavlja centralizirano mesto za delo z vsemi artefakti, ki jih ustvarite pri uporabi Azure Machine Learning. Delovni prostor vodi zgodovino vseh usposabljanj, vključno z dnevniki, metrikami, izhodom in posnetkom vaših skriptov. Te informacije uporabite za določitev, katero usposabljanje ustvari najboljši model. [Več o tem](https://docs.microsoft.com/azure/machine-learning/concept-workspace?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109)

Priporočljivo je, da uporabljate najbolj posodobljen brskalnik, ki je združljiv z vašim operacijskim sistemom. Podprti so naslednji brskalniki:

- Microsoft Edge (novi Microsoft Edge, najnovejša različica. Ne Microsoft Edge legacy)
- Safari (najnovejša različica, samo Mac)
- Chrome (najnovejša različica)
- Firefox (najnovejša različica)

Za uporabo Azure Machine Learning ustvarite delovni prostor v svoji naročnini Azure. Nato lahko ta delovni prostor uporabite za upravljanje podatkov, računalniških virov, kode, modelov in drugih artefaktov, povezanih z vašimi delovnimi obremenitvami strojnega učenja.

> **_OPOMBA:_** Vaša naročnina Azure bo zaračunana majhna količina za shranjevanje podatkov, dokler delovni prostor Azure Machine Learning obstaja v vaši naročnini, zato priporočamo, da izbrišete delovni prostor Azure Machine Learning, ko ga ne uporabljate več.

1. Prijavite se v [Azure portal](https://ms.portal.azure.com/) z Microsoftovimi poverilnicami, povezanimi z vašo naročnino Azure.
2. Izberite **＋Ustvari vir**
   
   ![workspace-1](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/workspace-1.PNG)

   Poiščite Machine Learning in izberite ploščico Machine Learning

   ![workspace-2](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/workspace-2.PNG)

   Kliknite gumb za ustvarjanje

   ![workspace-3](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/workspace-3.PNG)

   Izpolnite nastavitve, kot sledi:
   - Naročnina: Vaša naročnina Azure
   - Skupina virov: Ustvarite ali izberite skupino virov
   - Ime delovnega prostora: Vnesite edinstveno ime za vaš delovni prostor
   - Regija: Izberite geografsko regijo, ki je najbližja vam
   - Račun za shranjevanje: Upoštevajte privzeti nov račun za shranjevanje, ki bo ustvarjen za vaš delovni prostor
   - Key vault: Upoštevajte privzeti nov key vault, ki bo ustvarjen za vaš delovni prostor
   - Application insights: Upoštevajte privzeti nov vir za application insights, ki bo ustvarjen za vaš delovni prostor
   - Container registry: Noben (eden bo samodejno ustvarjen prvič, ko boste uvedli model v vsebnik)

    ![workspace-4](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/workspace-4.PNG)

   - Kliknite gumb za pregled in nato gumb za ustvarjanje
3. Počakajte, da se vaš delovni prostor ustvari (to lahko traja nekaj minut). Nato pojdite nanj v portalu. Najdete ga lahko prek storitve Machine Learning Azure.
4. Na strani Pregled za vaš delovni prostor zaženite Azure Machine Learning studio (ali odprite nov zavihek brskalnika in pojdite na https://ml.azure.com), ter se prijavite v Azure Machine Learning studio z Microsoftovim računom. Če ste pozvani, izberite svoj Azure imenik in naročnino ter svoj delovni prostor Azure Machine Learning.
   
![workspace-5](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/workspace-5.PNG)

5. V Azure Machine Learning studio preklopite ikono ☰ na vrhu levo, da si ogledate različne strani vmesnika. Te strani lahko uporabite za upravljanje virov v vašem delovnem prostoru.

![workspace-6](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/workspace-6.PNG)

Delovni prostor lahko upravljate z Azure portalom, vendar za podatkovne znanstvenike in inženirje operacij strojnega učenja Azure Machine Learning Studio ponuja bolj osredotočen uporabniški vmesnik za upravljanje virov delovnega prostora.

### 2.2 Računalniški viri

Računalniški viri so viri v oblaku, na katerih lahko izvajate procese usposabljanja modelov in raziskovanja podatkov. Obstajajo štiri vrste računalniških virov, ki jih lahko ustvarite:

- **Računalniški primerki**: Razvojne delovne postaje, ki jih podatkovni znanstveniki lahko uporabljajo za delo s podatki in modeli. To vključuje ustvarjanje virtualnega računalnika (VM) in zagon primerka beležke. Nato lahko usposobite model z uporabo računalniškega grozda iz beležke.
- **Računalniški grozdi**: Prilagodljivi grozdi VM za procesiranje eksperimentne kode na zahtevo. Potrebovali jih boste pri usposabljanju modela. Računalniški grozdi lahko uporabljajo tudi specializirane GPU ali CPU vire.
- **Inferenčni grozdi**: Cilji za uvajanje napovednih storitev, ki uporabljajo vaše usposobljene modele.
- **Priključeni računalniški viri**: Povezave do obstoječih Azure računalniških virov, kot so virtualni stroji ali Azure Databricks grozdi.

#### 2.2.1 Izbira pravih možnosti za vaše računalniške vire

Pri ustvarjanju računalniškega vira je treba upoštevati nekaj ključnih dejavnikov, saj so te odločitve lahko ključne.

**Ali potrebujete CPU ali GPU?**

CPU (Centralna procesna enota) je elektronsko vezje, ki izvaja navodila računalniškega programa. GPU (Grafična procesna enota) je specializirano elektronsko vezje, ki lahko izvaja grafično povezano kodo z zelo visoko hitrostjo.

Glavna razlika med arhitekturo CPU in GPU je, da je CPU zasnovan za hitro obdelavo širokega spektra nalog (merjeno s hitrostjo ure CPU), vendar je omejen pri sočasnem izvajanju nalog. GPU-ji so zasnovani za paralelno računalništvo in so zato veliko boljši pri nalogah globokega učenja.

| CPU                                     | GPU                         |
|-----------------------------------------|-----------------------------|
| Manj drago                              | Bolj drago                  |
| Nižja stopnja sočasnosti                | Višja stopnja sočasnosti    |
| Počasnejše pri učenju modelov globokega učenja | Optimalno za globoko učenje |

**Velikost grozda**

Večji grozdi so dražji, vendar zagotavljajo boljšo odzivnost. Če imate čas, vendar omejen proračun, začnite z majhnim grozdom. Če imate denar, vendar malo časa, začnite z večjim grozdom.

**Velikost VM**

Glede na vaše časovne in proračunske omejitve lahko prilagodite velikost RAM-a, diska, število jeder in hitrost ure. Povečanje vseh teh parametrov bo dražje, vendar bo prineslo boljšo zmogljivost.

**Namenske ali nizkoprioritetne instance?**

Nizkoprioritetna instanca pomeni, da je prekinljiva: Microsoft Azure lahko te vire dodeli drugi nalogi, kar prekine trenutno nalogo. Namenska instanca, ali neprekinljiva, pomeni, da naloga ne bo nikoli prekinjena brez vašega dovoljenja. To je še ena odločitev med časom in denarjem, saj so prekinljive instance cenejše od namenskih.

#### 2.2.2 Ustvarjanje računalniškega grozda

V [Azure ML delovnem prostoru](https://ml.azure.com/), ki smo ga ustvarili prej, pojdite na "Compute" in videli boste različne računalniške vire, o katerih smo pravkar razpravljali (tj. računalniške instance, računalniške grozde, grozde za sklepanje in priključene računalnike). Za ta projekt bomo potrebovali računalniški grozd za učenje modela. V Studio kliknite na meni "Compute", nato na zavihek "Compute cluster" in kliknite na gumb "+ New" za ustvarjanje računalniškega grozda.

![22](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/cluster-1.PNG)

1. Izberite svoje možnosti: Namensko ali nizkoprioritetno, CPU ali GPU, velikost VM in število jeder (za ta projekt lahko obdržite privzete nastavitve).
2. Kliknite na gumb "Next".

![23](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/cluster-2.PNG)

3. Dajte grozdu ime.
4. Izberite svoje možnosti: Minimalno/maksimalno število vozlišč, število sekund neaktivnosti pred zmanjšanjem obsega, SSH dostop. Upoštevajte, da če je minimalno število vozlišč 0, boste prihranili denar, ko je grozd neaktiven. Upoštevajte, da večje število maksimalnih vozlišč pomeni krajši čas učenja. Priporočeno maksimalno število vozlišč je 3.  
5. Kliknite na gumb "Create". Ta korak lahko traja nekaj minut.

![29](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/cluster-3.PNG)

Odlično! Zdaj, ko imamo računalniški grozd, moramo naložiti podatke v Azure ML Studio.

### 2.3 Nalaganje podatkovne zbirke

1. V [Azure ML delovnem prostoru](https://ml.azure.com/), ki smo ga ustvarili prej, kliknite na "Datasets" v levem meniju in kliknite na gumb "+ Create dataset" za ustvarjanje podatkovne zbirke. Izberite možnost "From local files" in izberite Kaggle podatkovno zbirko, ki smo jo prenesli prej.
   
   ![24](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/dataset-1.PNG)

2. Dajte podatkovni zbirki ime, vrsto in opis. Kliknite "Next". Naložite podatke iz datotek. Kliknite "Next".
   
   ![25](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/dataset-2.PNG)

3. V shemi spremenite vrsto podatkov v Boolean za naslednje značilnosti: anemija, diabetes, visok krvni tlak, spol, kajenje in DEATH_EVENT. Kliknite "Next" in nato "Create".
   
   ![26](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/dataset-3.PNG)

Odlično! Zdaj, ko je podatkovna zbirka na mestu in je računalniški grozd ustvarjen, lahko začnemo z učenjem modela!

### 2.4 Učenje z malo kode/brez kode z AutoML

Tradicionalni razvoj modelov strojnega učenja je zahteven, zahteva veliko domenskega znanja in časa za izdelavo ter primerjavo številnih modelov. 
Avtomatizirano strojno učenje (AutoML) je proces avtomatizacije časovno zahtevnih, ponavljajočih se nalog razvoja modelov strojnega učenja. Omogoča podatkovnim znanstvenikom, analitikom in razvijalcem, da gradijo modele strojnega učenja z visoko učinkovitostjo in produktivnostjo, hkrati pa ohranjajo kakovost modelov. Zmanjšuje čas, potreben za pridobitev modelov, pripravljenih za produkcijo, z veliko lahkoto in učinkovitostjo. [Več o tem](https://docs.microsoft.com/azure/machine-learning/concept-automated-ml?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109)

1. V [Azure ML delovnem prostoru](https://ml.azure.com/), ki smo ga ustvarili prej, kliknite na "Automated ML" v levem meniju in izberite podatkovno zbirko, ki ste jo pravkar naložili. Kliknite "Next".

   ![27](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/aml-1.PNG)

2. Vnesite ime novega eksperimenta, ciljni stolpec (DEATH_EVENT) in računalniški grozd, ki smo ga ustvarili. Kliknite "Next".
   
   ![28](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/aml-2.PNG)

3. Izberite "Classification" in kliknite "Finish". Ta korak lahko traja med 30 minutami in 1 uro, odvisno od velikosti vašega računalniškega grozda.
    
    ![30](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/aml-3.PNG)

4. Ko je postopek končan, kliknite na zavihek "Automated ML", kliknite na svoj postopek in nato na algoritem v kartici "Best model summary".
    
    ![31](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/aml-4.PNG)

Tukaj lahko vidite podroben opis najboljšega modela, ki ga je AutoML ustvaril. Prav tako lahko raziščete druge modele v zavihku "Models". Vzemite si nekaj minut za raziskovanje modelov v razlagah (gumb za predogled). Ko izberete model, ki ga želite uporabiti (tukaj bomo izbrali najboljši model, ki ga je izbral AutoML), bomo videli, kako ga lahko namestimo.

## 3. Namestitev modela z malo kode/brez kode in uporaba končne točke
### 3.1 Namestitev modela

Vmesnik avtomatiziranega strojnega učenja omogoča namestitev najboljšega modela kot spletne storitve v nekaj korakih. Namestitev je integracija modela, da lahko na podlagi novih podatkov napoveduje in identificira potencialna področja priložnosti. Za ta projekt namestitev v spletno storitev pomeni, da bodo medicinske aplikacije lahko uporabljale model za izdelavo živih napovedi tveganja za srčni napad pri svojih pacientih.

V opisu najboljšega modela kliknite na gumb "Deploy".
    
![deploy-1](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/deploy-1.PNG)

15. Dajte mu ime, opis, vrsto računalnika (Azure Container Instance), omogočite avtentikacijo in kliknite na "Deploy". Ta korak lahko traja približno 20 minut. Postopek namestitve vključuje več korakov, vključno z registracijo modela, ustvarjanjem virov in njihovo konfiguracijo za spletno storitev. Status se prikaže pod "Deploy status". Občasno kliknite "Refresh", da preverite status namestitve. Ko je status "Healthy", je model nameščen in deluje.

![deploy-2](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/deploy-2.PNG)

16. Ko je nameščen, kliknite na zavihek "Endpoint" in kliknite na končno točko, ki ste jo pravkar namestili. Tukaj lahko najdete vse podrobnosti o končni točki.

![deploy-3](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/deploy-3.PNG)

Odlično! Zdaj, ko imamo nameščen model, lahko začnemo z uporabo končne točke.

### 3.2 Uporaba končne točke

Kliknite na zavihek "Consume". Tukaj lahko najdete REST končno točko in Python skripto v možnosti uporabe. Vzemite si čas za pregled Python kode.

Ta skripta se lahko zažene neposredno z vašega lokalnega računalnika in bo uporabila vašo končno točko.

![35](../../../../5-Data-Science-In-Cloud/18-Low-Code/images/consumption-1.PNG)

Vzemite si trenutek za pregled teh dveh vrstic kode:

```python
url = 'http://98e3715f-xxxx-xxxx-xxxx-9ec22d57b796.centralus.azurecontainer.io/score'
api_key = '' # Replace this with the API key for the web service
```
Spremenljivka `url` je REST končna točka, ki jo najdete v zavihku "Consume", in spremenljivka `api_key` je primarni ključ, ki ga prav tako najdete v zavihku "Consume" (samo v primeru, da ste omogočili avtentikacijo). Tako skripta lahko uporabi končno točko.

18. Ko zaženete skripto, bi morali videti naslednji izhod:
    ```python
    b'"{\\"result\\": [true]}"'
    ```
To pomeni, da je napoved srčnega popuščanja za podane podatke resnična. To je smiselno, saj če podrobneje pogledate podatke, ki jih je skripta samodejno generirala, je vse privzeto nastavljeno na 0 in napačno. Podatke lahko spremenite z naslednjim vzorcem vnosa:

```python
data = {
    "data":
    [
        {
            'age': "0",
            'anaemia': "false",
            'creatinine_phosphokinase': "0",
            'diabetes': "false",
            'ejection_fraction': "0",
            'high_blood_pressure': "false",
            'platelets': "0",
            'serum_creatinine': "0",
            'serum_sodium': "0",
            'sex': "false",
            'smoking': "false",
            'time': "0",
        },
        {
            'age': "60",
            'anaemia': "false",
            'creatinine_phosphokinase': "500",
            'diabetes': "false",
            'ejection_fraction': "38",
            'high_blood_pressure': "false",
            'platelets': "260000",
            'serum_creatinine': "1.40",
            'serum_sodium': "137",
            'sex': "false",
            'smoking': "false",
            'time': "130",
        },
    ],
}
```
Skripta bi morala vrniti:
    ```python
    b'"{\\"result\\": [true, false]}"'
    ```

Čestitke! Pravkar ste uporabili model, ki ste ga namestili in ga naučili na Azure ML!

> **_OPOMBA:_** Ko končate projekt, ne pozabite izbrisati vseh virov.
## 🚀 Izziv

Podrobno preglejte razlage modelov in podrobnosti, ki jih je AutoML ustvaril za najboljše modele. Poskusite razumeti, zakaj je najboljši model boljši od drugih. Katere algoritme so primerjali? Kakšne so razlike med njimi? Zakaj je najboljši model v tem primeru boljši?

## [Kvizi po predavanju](https://ff-quizzes.netlify.app/en/ds/)

## Pregled in samostojno učenje

V tej lekciji ste se naučili, kako naučiti, namestiti in uporabiti model za napovedovanje tveganja srčnega popuščanja na način z malo kode/brez kode v oblaku. Če tega še niste storili, se poglobite v razlage modelov, ki jih je AutoML ustvaril za najboljše modele, in poskusite razumeti, zakaj je najboljši model boljši od drugih.

Lahko se poglobite v AutoML z malo kode/brez kode z branjem te [dokumentacije](https://docs.microsoft.com/azure/machine-learning/tutorial-first-experiment-automated-ml?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109).

## Naloga

[Projekt podatkovne znanosti z malo kode/brez kode na Azure ML](assignment.md)

---

**Omejitev odgovornosti**:  
Ta dokument je bil preveden z uporabo storitve za prevajanje z umetno inteligenco [Co-op Translator](https://github.com/Azure/co-op-translator). Čeprav si prizadevamo za natančnost, vas prosimo, da upoštevate, da lahko avtomatizirani prevodi vsebujejo napake ali netočnosti. Izvirni dokument v njegovem maternem jeziku je treba obravnavati kot avtoritativni vir. Za ključne informacije priporočamo profesionalni človeški prevod. Ne prevzemamo odgovornosti za morebitna napačna razumevanja ali napačne interpretacije, ki bi nastale zaradi uporabe tega prevoda.