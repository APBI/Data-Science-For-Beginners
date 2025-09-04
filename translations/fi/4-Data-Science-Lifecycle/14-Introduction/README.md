<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "79ca8a5a3135e94d2d43f56ba62d5205",
  "translation_date": "2025-09-04T19:40:57+00:00",
  "source_file": "4-Data-Science-Lifecycle/14-Introduction/README.md",
  "language_code": "fi"
}
-->
# Johdanto datatieteen elinkaareen

|![ Sketchnote by [(@sketchthedocs)](https://sketchthedocs.dev) ](../../sketchnotes/14-DataScience-Lifecycle.png)|
|:---:|
| Johdanto datatieteen elinkaareen - _Sketchnote by [@nitya](https://twitter.com/nitya)_ |

## [Ennen luentoa - kysely](https://red-water-0103e7a0f.azurestaticapps.net/quiz/26)

Olet luultavasti jo huomannut, että datatiede on prosessi. Tämä prosessi voidaan jakaa viiteen vaiheeseen:

- Tiedon kerääminen
- Tiedon käsittely
- Analyysi
- Viestintä
- Ylläpito

Tämä oppitunti keskittyy elinkaaren kolmeen osaan: tiedon keräämiseen, käsittelyyn ja ylläpitoon.

![Datatieteen elinkaaren kaavio](../../../../translated_images/data-science-lifecycle.a1e362637503c4fb0cd5e859d7552edcdb4aa629a279727008baa121f2d33f32.fi.jpg)
> Kuva: [Berkeley School of Information](https://ischoolonline.berkeley.edu/data-science/what-is-data-science/)

## Tiedon kerääminen

Elinkaaren ensimmäinen vaihe on erittäin tärkeä, sillä seuraavat vaiheet riippuvat siitä. Käytännössä tämä vaihe yhdistää kaksi osaa: tiedon hankkimisen sekä projektin tarkoituksen ja ratkaistavien ongelmien määrittelyn.  
Projektin tavoitteiden määrittely vaatii syvempää ymmärrystä ongelmasta tai kysymyksestä. Ensimmäiseksi meidän täytyy tunnistaa ja hankkia ne, joiden ongelma tarvitsee ratkaisua. Nämä voivat olla yrityksen sidosryhmiä tai projektin sponsoreita, jotka voivat auttaa tunnistamaan, kuka tai mikä hyötyy projektista, sekä mitä ja miksi he sitä tarvitsevat. Hyvin määritelty tavoite tulisi olla mitattavissa ja kvantifioitavissa, jotta hyväksyttävä tulos voidaan määrittää.

Kysymyksiä, joita datatieteilijä saattaa kysyä:
- Onko tätä ongelmaa lähestytty aiemmin? Mitä havaittiin?
- Ymmärtävätkö kaikki osapuolet tarkoituksen ja tavoitteen?
- Onko epäselvyyksiä, ja miten niitä voidaan vähentää?
- Mitkä ovat rajoitteet?
- Miltä lopputulos mahdollisesti näyttää?
- Kuinka paljon resursseja (aikaa, ihmisiä, laskentatehoa) on käytettävissä?

Seuraavaksi tunnistetaan, kerätään ja lopulta tutkitaan dataa, joka tarvitaan näiden tavoitteiden saavuttamiseksi. Tiedon hankinnan tässä vaiheessa datatieteilijöiden täytyy myös arvioida datan määrä ja laatu. Tämä vaatii jonkin verran datan tutkimista, jotta voidaan varmistaa, että hankittu data tukee halutun tuloksen saavuttamista.

Kysymyksiä, joita datatieteilijä saattaa kysyä datasta:
- Mitä dataa minulla on jo saatavilla?
- Kuka omistaa tämän datan?
- Mitä yksityisyysongelmia on olemassa?
- Onko minulla tarpeeksi dataa tämän ongelman ratkaisemiseksi?
- Onko data riittävän laadukasta tähän ongelmaan?
- Jos löydän lisätietoa datan kautta, pitäisikö meidän harkita tavoitteiden muuttamista tai uudelleenmäärittelyä?

## Tiedon käsittely

Elinkaaren käsittelyvaihe keskittyy datan kuvioiden löytämiseen sekä mallintamiseen. Joitakin käsittelyvaiheessa käytettyjä tekniikoita ovat tilastolliset menetelmät, jotka paljastavat datan kuvioita. Tyypillisesti tämä olisi ihmiselle työläs tehtävä suuren datamäärän kanssa, ja siksi tietokoneet tekevät raskaan työn prosessin nopeuttamiseksi. Tämä vaihe on myös se, missä datatiede ja koneoppiminen kohtaavat. Kuten opit ensimmäisessä oppitunnissa, koneoppiminen on prosessi, jossa rakennetaan malleja datan ymmärtämiseksi. Mallit ovat datan muuttujien välisten suhteiden esityksiä, jotka auttavat ennustamaan tuloksia.

Yleisiä tekniikoita, joita tässä vaiheessa käytetään, käsitellään ML for Beginners -opetussuunnitelmassa. Seuraa linkkejä oppiaksesi lisää:

- [Luokittelu](https://github.com/microsoft/ML-For-Beginners/tree/main/4-Classification): Datan järjestäminen kategorioihin tehokkaampaa käyttöä varten.
- [Klusterointi](https://github.com/microsoft/ML-For-Beginners/tree/main/5-Clustering): Datan ryhmittely samankaltaisiin ryhmiin.
- [Regressio](https://github.com/microsoft/ML-For-Beginners/tree/main/2-Regression): Muuttujien välisten suhteiden määrittäminen arvojen ennustamiseksi tai arvioimiseksi.

## Ylläpito

Elinkaaren kaaviossa saatat huomata, että ylläpito sijoittuu tiedon keräämisen ja käsittelyn väliin. Ylläpito on jatkuva prosessi, jossa hallitaan, tallennetaan ja suojataan dataa projektin aikana, ja se tulisi ottaa huomioon projektin koko keston ajan.

### Datan tallentaminen

Päätökset siitä, miten ja missä data tallennetaan, voivat vaikuttaa tallennuskustannuksiin sekä siihen, kuinka nopeasti dataa voidaan käyttää. Tällaisia päätöksiä ei todennäköisesti tee datatieteilijä yksin, mutta hän saattaa joutua tekemään valintoja siitä, miten dataa käsitellään sen tallennustavan perusteella.

Tässä joitakin nykyaikaisten datan tallennusjärjestelmien ominaisuuksia, jotka voivat vaikuttaa näihin valintoihin:

**Paikallinen vs ulkoinen vs julkinen tai yksityinen pilvi**

Paikallinen viittaa datan hallintaan omalla laitteistolla, kuten palvelimella, jossa data tallennetaan kiintolevyille. Ulkoinen tallennus taas käyttää laitteistoa, jota et omista, kuten datakeskusta. Julkinen pilvi on suosittu valinta datan tallentamiseen, joka ei vaadi tietoa siitä, miten tai missä data tarkalleen ottaen tallennetaan. Julkinen viittaa yhtenäiseen infrastruktuuriin, jota kaikki pilven käyttäjät jakavat. Joillakin organisaatioilla on tiukat turvallisuuspolitiikat, jotka vaativat täydellisen pääsyn laitteistoon, jossa dataa isännöidään, ja he käyttävät yksityistä pilveä, joka tarjoaa omat pilvipalvelut. Opit lisää datasta pilvessä [myöhemmissä oppitunneissa](https://github.com/microsoft/Data-Science-For-Beginners/tree/main/5-Data-Science-In-Cloud).

**Kylmä vs kuuma data**

Kun koulutat mallejasi, saatat tarvita enemmän koulutusdataa. Jos olet tyytyväinen mallisi toimintaan, lisää dataa saapuu mallin tarkoituksen täyttämiseksi. Joka tapauksessa datan tallennus- ja käyttömahdollisuuksien kustannukset kasvavat datan määrän kasvaessa. Harvoin käytetyn datan, eli kylmän datan, erottaminen usein käytetystä kuumasta datasta voi olla edullisempi tallennusvaihtoehto laitteiston tai ohjelmistopalveluiden avulla. Jos kylmää dataa täytyy käyttää, sen hakeminen voi kestää hieman kauemmin verrattuna kuumaan dataan.

### Datan hallinta

Työskennellessäsi datan kanssa saatat huomata, että osa datasta täytyy puhdistaa käyttämällä joitakin tekniikoita, jotka käsitellään oppitunnissa, joka keskittyy [datan valmisteluun](https://github.com/microsoft/Data-Science-For-Beginners/tree/main/2-Working-With-Data/08-data-preparation), jotta voidaan rakentaa tarkkoja malleja. Kun uutta dataa saapuu, se tarvitsee samoja sovelluksia laadun yhdenmukaisuuden ylläpitämiseksi. Joissakin projekteissa käytetään automatisoituja työkaluja datan puhdistamiseen, yhdistämiseen ja pakkaamiseen ennen kuin data siirretään lopulliseen sijaintiinsa. Azure Data Factory on esimerkki tällaisesta työkalusta.

### Datan suojaaminen

Yksi datan suojaamisen päämääristä on varmistaa, että datan kanssa työskentelevät hallitsevat, mitä kerätään ja missä kontekstissa sitä käytetään. Datan suojaaminen sisältää pääsyn rajoittamisen vain niille, jotka sitä tarvitsevat, paikallisten lakien ja säädösten noudattamisen sekä eettisten standardien ylläpitämisen, kuten käsitellään [etiikkaa käsittelevässä oppitunnissa](https://github.com/microsoft/Data-Science-For-Beginners/tree/main/1-Introduction/02-ethics).

Tässä joitakin asioita, joita tiimi saattaa tehdä turvallisuuden huomioimiseksi:
- Varmistaa, että kaikki data on salattu
- Tarjota asiakkaille tietoa siitä, miten heidän dataansa käytetään
- Poistaa datan käyttöoikeudet niiltä, jotka ovat poistuneet projektista
- Sallia vain tiettyjen projektin jäsenten muokata dataa

## 🚀 Haaste

Datatieteen elinkaaresta on monia versioita, joissa jokaisella vaiheella voi olla eri nimet ja eri määrä vaiheita, mutta ne sisältävät samat prosessit, jotka mainittiin tässä oppitunnissa.

Tutki [Team Data Science Process -elinkaarta](https://docs.microsoft.com/en-us/azure/architecture/data-science-process/lifecycle) ja [Cross-industry standard process for data mining](https://www.datascience-pm.com/crisp-dm-2/). Nimeä kolme yhtäläisyyttä ja eroa näiden kahden välillä.

|Team Data Science Process (TDSP)|Cross-industry standard process for data mining (CRISP-DM)|
|--|--|
|![Team Data Science Lifecycle](../../../../translated_images/tdsp-lifecycle2.e19029d598e2e73d5ef8a4b98837d688ec6044fe332c905d4dbb69eb6d5c1d96.fi.png) | ![Data Science Process Alliance Image](../../../../translated_images/CRISP-DM.8bad2b4c66e62aa75278009e38e3e99902c73b0a6f63fd605a67c687a536698c.fi.png) |
| Kuva: [Microsoft](https://docs.microsoft.comazure/architecture/data-science-process/lifecycle) | Kuva: [Data Science Process Alliance](https://www.datascience-pm.com/crisp-dm-2/) |

## [Luentojälkeinen kysely](https://ff-quizzes.netlify.app/en/ds/)

## Kertaus ja itseopiskelu

Datatieteen elinkaaren soveltaminen sisältää useita rooleja ja tehtäviä, joissa jotkut keskittyvät tiettyihin osiin jokaisesta vaiheesta. Team Data Science Process tarjoaa muutamia resursseja, jotka selittävät rooleja ja tehtäviä, joita joku saattaa projektissa hoitaa.

* [Team Data Science Process -roolit ja tehtävät](https://docs.microsoft.com/en-us/azure/architecture/data-science-process/roles-tasks)
* [Datatieteen tehtävien suorittaminen: tutkiminen, mallintaminen ja käyttöönotto](https://docs.microsoft.com/en-us/azure/architecture/data-science-process/execute-data-science-tasks)

## Tehtävä

[Datasetin arviointi](assignment.md)

---

**Vastuuvapauslauseke**:  
Tämä asiakirja on käännetty käyttämällä tekoälypohjaista käännöspalvelua [Co-op Translator](https://github.com/Azure/co-op-translator). Vaikka pyrimme tarkkuuteen, huomioithan, että automaattiset käännökset voivat sisältää virheitä tai epätarkkuuksia. Alkuperäistä asiakirjaa sen alkuperäisellä kielellä tulisi pitää ensisijaisena lähteenä. Kriittisen tiedon osalta suositellaan ammattimaista ihmiskäännöstä. Emme ole vastuussa väärinkäsityksistä tai virhetulkinnoista, jotka johtuvat tämän käännöksen käytöstä.