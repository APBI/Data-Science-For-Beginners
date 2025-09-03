<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "8141e7195841682914be03ef930fe43d",
  "translation_date": "2025-09-03T20:28:23+00:00",
  "source_file": "1-Introduction/01-defining-data-science/README.md",
  "language_code": "sk"
}
-->
## Typy dát

Ako sme už spomenuli, dáta sú všade. Stačí ich len správne zachytiť! Je užitočné rozlišovať medzi **štruktúrovanými** a **neštruktúrovanými** dátami. Štruktúrované dáta sú zvyčajne reprezentované v nejakej dobre štruktúrovanej forme, často ako tabuľka alebo množstvo tabuliek, zatiaľ čo neštruktúrované dáta sú len zbierkou súborov. Niekedy môžeme hovoriť aj o **pološtruktúrovaných** dátach, ktoré majú určitý druh štruktúry, ktorá sa môže značne líšiť.

| Štruktúrované                                                              | Pološtruktúrované                                                                            | Neštruktúrované                        |
| -------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | -------------------------------------- |
| Zoznam ľudí s ich telefónnymi číslami                                      | Stránky Wikipédie s odkazmi                                                                 | Text Encyklopédie Britannica          |
| Teplota vo všetkých miestnostiach budovy každú minútu za posledných 20 rokov | Zbierka vedeckých článkov vo formáte JSON s autormi, dátumom publikácie a abstraktom         | Zdieľané súbory s firemnými dokumentmi |
| Dáta o veku a pohlaví všetkých ľudí vstupujúcich do budovy                 | Internetové stránky                                                                         | Surový videozáznam z bezpečnostnej kamery |

## Kde získať dáta

Existuje mnoho možných zdrojov dát, a bolo by nemožné ich všetky vymenovať! Avšak, spomeňme niektoré typické miesta, kde môžete získať dáta:

* **Štruktúrované**
  - **Internet vecí** (IoT), vrátane dát z rôznych senzorov, ako sú senzory teploty alebo tlaku, poskytuje množstvo užitočných dát. Napríklad, ak je kancelárska budova vybavená IoT senzormi, môžeme automaticky riadiť kúrenie a osvetlenie, aby sme minimalizovali náklady.
  - **Prieskumy**, ktoré žiadame používateľov vyplniť po nákupe alebo po návšteve webovej stránky.
  - **Analýza správania** nám môže napríklad pomôcť pochopiť, ako hlboko sa používateľ dostane na stránku a aký je typický dôvod jej opustenia.
* **Neštruktúrované**
  - **Texty** môžu byť bohatým zdrojom poznatkov, ako napríklad celkový **sentiment skóre** alebo extrakcia kľúčových slov a sémantického významu.
  - **Obrázky** alebo **video**. Video z bezpečnostnej kamery môže byť použité na odhad dopravnej situácie na ceste a informovanie ľudí o možných dopravných zápchach.
  - **Logy** webového servera môžu byť použité na pochopenie, ktoré stránky našej webovej stránky sú najčastejšie navštevované a ako dlho.
* Pološtruktúrované
  - **Grafy sociálnych sietí** môžu byť skvelým zdrojom dát o osobnostiach používateľov a potenciálnej efektivite šírenia informácií.
  - Keď máme množstvo fotografií z večierka, môžeme sa pokúsiť extrahovať dáta o **skupinovej dynamike** vytvorením grafu ľudí, ktorí sa fotili spolu.

Poznaním rôznych možných zdrojov dát môžete premýšľať o rôznych scenároch, kde je možné aplikovať techniky dátovej vedy na lepšie pochopenie situácie a zlepšenie obchodných procesov.

## Čo môžete robiť s dátami

V dátovej vede sa zameriavame na nasledujúce kroky v práci s dátami:

Samozrejme, v závislosti od konkrétnych dát môžu niektoré kroky chýbať (napr. keď už máme dáta v databáze alebo keď nepotrebujeme trénovať model), alebo niektoré kroky môžu byť opakované viackrát (napríklad spracovanie dát).

## Digitalizácia a digitálna transformácia

V poslednom desaťročí si mnoho firiem začalo uvedomovať dôležitosť dát pri rozhodovaní o podnikaní. Aby bolo možné aplikovať princípy dátovej vedy na riadenie podnikania, je najprv potrebné zhromaždiť nejaké dáta, teda preložiť obchodné procesy do digitálnej formy. Toto sa nazýva **digitalizácia**. Aplikácia techník dátovej vedy na tieto dáta na podporu rozhodovania môže viesť k významnému zvýšeniu produktivity (alebo dokonca k zmene podnikania), čo sa nazýva **digitálna transformácia**.

Pozrime sa na príklad. Predpokladajme, že máme kurz dátovej vedy (ako tento), ktorý poskytujeme online študentom, a chceme ho pomocou dátovej vedy zlepšiť. Ako to môžeme urobiť?

Môžeme začať otázkou „Čo sa dá digitalizovať?“ Najjednoduchší spôsob by bol merať čas, ktorý každý študent potrebuje na dokončenie každého modulu, a merať získané vedomosti pomocou testu s výberom odpovedí na konci každého modulu. Priemerovaním času na dokončenie medzi všetkými študentmi môžeme zistiť, ktoré moduly spôsobujú študentom najväčšie ťažkosti, a pracovať na ich zjednodušení.
Môžete namietať, že tento prístup nie je ideálny, pretože moduly môžu mať rôznu dĺžku. Pravdepodobne by bolo spravodlivejšie rozdeliť čas podľa dĺžky modulu (v počte znakov) a porovnať tieto hodnoty namiesto toho.
Keď začneme analyzovať výsledky testov s výberom odpovede, môžeme sa pokúsiť určiť, ktoré koncepty robia študentom problémy, a využiť tieto informácie na zlepšenie obsahu. Aby sme to dosiahli, musíme navrhnúť testy tak, aby každá otázka zodpovedala určitému konceptu alebo časti vedomostí.

Ak chceme ísť ešte hlbšie, môžeme porovnať čas potrebný na dokončenie jednotlivých modulov s vekovou kategóriou študentov. Môžeme zistiť, že pre niektoré vekové kategórie trvá dokončenie modulu neprimerane dlho, alebo že študenti modul nedokončia. To nám môže pomôcť poskytnúť vekové odporúčania pre modul a minimalizovať nespokojnosť ľudí spôsobenú nesprávnymi očakávaniami.

## 🚀 Výzva

V tejto výzve sa pokúsime nájsť koncepty relevantné pre oblasť dátovej vedy analýzou textov. Vezmeme si článok z Wikipédie o dátovej vede, stiahneme a spracujeme text a potom vytvoríme slovný mrak, ako je tento:

![Slovný mrak pre dátovú vedu](../../../../translated_images/ds_wordcloud.664a7c07dca57de017c22bf0498cb40f898d48aa85b3c36a80620fea12fadd42.sk.png)

Navštívte [`notebook.ipynb`](../../../../../../../../../1-Introduction/01-defining-data-science/notebook.ipynb ':ignore'), aby ste si prešli kód. Môžete tiež spustiť kód a sledovať, ako vykonáva všetky transformácie dát v reálnom čase.

> Ak neviete, ako spustiť kód v Jupyter Notebooku, pozrite si [tento článok](https://soshnikov.com/education/how-to-execute-notebooks-from-github/).

## [Kvíz po prednáške](https://ff-quizzes.netlify.app/en/ds/)

## Zadania

* **Úloha 1**: Upravte vyššie uvedený kód tak, aby ste našli súvisiace koncepty pre oblasti **Big Data** a **Machine Learning**
* **Úloha 2**: [Premýšľajte o scenároch dátovej vedy](assignment.md)

## Poďakovanie

Táto lekcia bola vytvorená s ♥️ [Dmitry Soshnikov](http://soshnikov.com)

---

**Upozornenie**:  
Tento dokument bol preložený pomocou služby AI prekladu [Co-op Translator](https://github.com/Azure/co-op-translator). Hoci sa snažíme o presnosť, prosím, berte na vedomie, že automatizované preklady môžu obsahovať chyby alebo nepresnosti. Pôvodný dokument v jeho rodnom jazyku by mal byť považovaný za autoritatívny zdroj. Pre kritické informácie sa odporúča profesionálny ľudský preklad. Nenesieme zodpovednosť za akékoľvek nedorozumenia alebo nesprávne interpretácie vyplývajúce z použitia tohto prekladu.