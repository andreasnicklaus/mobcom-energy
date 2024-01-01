---
marp: true

# theme: uncover
# class: invert

paginate: true
header: 'Umweltbelastung von Moderner Mobilkommunikation, Andreas Nicklaus, 08.01.2024'

lang: de
math: mathjax

style: |
  footer > a {
    color: #999;
    text-decoration: underline
  }
  img[alt~=center]{
    width: 100%;
    object-fit: contain;
    margin: auto;
  }
  footer {
    width: 90%;
  }
  section.centered * {
    text-align: center;
  }
  section.tableCenter table {
    margin: 0 auto;
  }
  section.smalltable table {
    font-size: 0.8em;
  }
---

<!--
_paginate: hide
_header: ''
_footer: ''
TODO: Vortragsnotizen machen
-->
# Umweltbelastung von Moderner Mobilkommunikation

*Spezielle Themen Mobiler Kommunikationssysteme*
*Andreas Nicklaus*


<!--

Hallo, willkommen zu meiner Vorstellung des Themas Umweltbelastung von Moderner Mobilkommunikation.
- nicht so festgenagelt oder sicher feststehend wie Max vor der Weihnachtspause
- mehr Idee, und Bedeutung und weniger Fachwissen, aber auch
-->
---

# Worum geht's heute?

1. Was ist Umweltbelastung?​
2. Wie stark ist der Einfluss von Mobilkommunikation auf die Umwelt?​
3. Wo kommt der Energieverbrauch her?​
4. Wie kann eingespart werden?​

<!-- 
Plan für die kommenden noch etwa 29 Minuten: 4 Fragen beantworten oder einführen

1. Was ist Umweltbelastung?
2. Wie stark ist die Umweltbelastung im Kontext der ersten Antwort?
3. Wo in der Mobilkommunikation, insbesondere in BS, kommt der Energieverbrauch her?
4. Interessantestes Thema am Ende, aber kurz, welche Strategien gibt es einzusparen?

a.k.a.:
1. Worüber reden wir, worüber nicht? Kriterien ohne Maß
2. Zahlen und Fakten zum Stromverbrauch
3. Wir verteilen sich die Zahlen?
4. Dieses Seminar: Spezielle Entwicklungen in der Mobilkommunikation im Themenbereich

 -->
--- 

# 1. Was ist Umweltbelastung?

<!--

Wenn es euch so geht, wie mir habt ihr zwar eine ungefähre Vorstellung von

- Effekt von Umweltbelastung
- schlimme Akteure bzgl. Umweltbelastung

Was zählt alles dazu außer der Kohlendioxidaustoß?

 -->

---

## Anwendbar: 10 von 27 Umweltindikatoren

| Klima und Energie        | Umwelt und Gesundheit​ | Ressourcen und Effizienz​     |
| ------------------------ | ---------------------- | ----------------------------- |
| Kohlendioxidemissionen ​ | Luftqualität​          | Verwertungsquote​             |
| Energieverbrauch         | Lärmbelastung​         | Ressourcenproduktivität​      |
| Erneuerbare Energien​    |                        | Siedlungs- und Verkehrsfläche |
|                          |                        | Flächenverbrauch​             |
|                          |                        | Altlasten​                    |

<!-- _footer: '["Alle Umweltindikatoren auf einen Blick", Bayerisches Landesamt für Umwelt, https://www.lfu.bayern.de/umweltdaten/indikatoren/liste_indikatoren/index.htm](https://www.lfu.bayern.de/umweltdaten/indikatoren/liste_indikatoren/index.htm)' -->

<!-- 
Das Bayerische Landesamt für Umwelt hat unsere Arbeit dahingehend getan, dass sie 27 Indikatoren für die Umweltbelastung festgelegt haben.
- Indikatoren, nicht Kriterien -> nicht schlecht, weil es zutrifft, sondern in Kombination
- -> Beispiel bringen

10 von den 27 sind interessant:

Klima und Energie (wenig überraschend)
Umwelt und Gesundheit (wenig überraschend)
Ressourcen und Effizienz (wenn etwas mal steht und funktioniert, wie lange und kann es wiederverwendet werden)

Info: 9 Indikatoren aus Natur und Landschaft treffen nicht zu

 -->

--- 

## Vernachlässigbare Umweltindikatoren

- Kohlendioxidemissionen
- Luftqualität
- Lärmbelastung
- Siedlungs- und Verkehrsfläche
- Flächenverbrauch
- Altlasten

<!-- 
Von den 10 Indikatoren, bei denen man sich vorstellen kann, dass sie zutreffend sein könnten, sind diese 6 erst mal vernachlässigbar.

Kohlendioxidemissionen und Luftqualität nur für Generator für  generelle Stromversorgung oder Notstromversorgung
Lärmbelastung genauso.
TODO: wie laut sind gNB Base Stations?

Siedlungs-und Verkehrsfläche und Flächenverbrauch schauen wir uns auf der nächsten Folie ganz kurz an.
Altlasten sind grob bleibende Schäden nach der Bebauung, hängen also eng mit der Baufläche zusammen.
-->
---

[![bg left](./bilder/LTE-Antenne-Halle-Neustadt.jpg)](https://www.telefonica.de/netze/mobilfunknetz/antennenstandorte.html)

> Für den Betrieb einer Funkstation auf dem Dach werden etwa **10 m²** Technikstellfläche, für einen Mast ungefähr **150 m²** Grundfläche bzw. Technikstellfläche benötigt.

<!-- _footer: '["Mobilfunkausbau unterstützen - Antennenstandort anbieten", Deutsche Funkturm, https://www.dfmg.de/de/ihr-standortangebot-an-uns/anmietung-von-flaechen.html](https://www.dfmg.de/de/ihr-standortangebot-an-uns/anmietung-von-flaechen.html)' -->

<!-- 
Wie sieht die Baufläche für eine Base Station aus?

[Foto] von LTE Antenne bei Halle Neustadt

Die Deutsche Funkturm, Unternehmen für den Ausbau von Infrastruktur für deutsche Mobilfunkanbieter, schreibt folgendes in die Ausschreibung für Standorte für Base Stations.

[Zitat]

Wir können daraus und etlichen Standorten erkennen, dass kaum neue Flächen für den Bau und Betrieb von Base Stations versiegelt werden müssen.
Die Siedlungs- und Verkehrsfläche, der Flächenverbrauch und die Altlasten sind also meiner Meinung nach weniger ein Thema für uns heute und mehr für Architekten und Stadtplaner, daher für jetzt mal vernachlässigbar.

 -->

---

## Relevante Umweltindikatoren

- Energieverbrauch
- Erneuerbare Energien
- Verwertungsquote
- Ressourcenproduktivität

<!-- 
Jetzt habe ich erfolgreich 6 von 10 Indikatoren hier als vernachlässigbar abgestempelt, also kommen wir bei den 4 Indikatoren an, mit denen wahrscheinlich ohnehin jeder gerechnet hat. :)

Energieverbrauch = Stromverbrauch
Erneuerbare Energien = Anteil an Strom von erneuerbaren Energiequellen
Verwertungsquote = Was kann wiederverwendet werden? erneuert / anders verwendet
Ressourcenproduktivität = erzielte Wirtschaftsleistung pro eingesetzter Ressourceneinheit

 -->

---

## Ressourcenproduktivität seit 1991
![h:500 center](bilder/Ressourcenproduktivität-DE.png)
<!-- _footer: '["Ressourcenproduktivität", Bayerisches Landesamt für Umwelt, https://www.lfu.bayern.de/umweltdaten/indikatoren/ressourcen_effizienz/ressourcenproduktivitaet/index.htm](https://www.lfu.bayern.de/umweltdaten/indikatoren/ressourcen_effizienz/ressourcenproduktivitaet/index.htm)' -->

<!-- 
Mir hat das nichts gesagt und es sagt auch als absoluter Wert nichts aus, sondern als relativer Wert.

[Foto] beschreiben, Trend

[Vertrösten, dass nicht mehr dazu kommt, aber angesprochen bei Batterien]

 -->

---

## Batterien in gNB Base Stations
*Verwertungsquote und Ressourcenproduktivität*

- Lithium-Ionen Batterien
- Lebenszeit:
  - von 2-3 Jahren (max. 10) oder
  - 500-1000 Ladungen (max. 6000)
- Wiederverwendung:
  - Nach 20-30% Kapazitätsverlust
  - Wiederaufbereitung oder Repurposing
  - 40% der Produktionskosten bei Wiederaufbereitung

<!-- _footer: '
["How Long Do Lithium-Ion Batteries Last?", Li Time, 8.5.2023, https://www.litime.com/blogs/blogs/how-long-do-lithium-ion-batteries-last](https://www.litime.com/blogs/blogs/how-long-do-lithium-ion-batteries-last)

[Toward Sustainable Reuse of Retired Lithium-ion Batteries from
Electric Vehicles, Conservation and Recycling,
Volume 168, 2021, Yang et al.](https://linkinghub.elsevier.com/retrieve/pii/S0921344920305644)'  -->

<!-- 
Wenn wir über die Batterien in next generation Base Stations sprechen, dann über die Leistung, was wir gleich vergleichen werden, aber insbesondere über die Lebensdauer und Wiederverwendung.

Eines der bekanntesten Batterientypen heute sind Lithium-Ionen Batterien, häufig in Verbindung gebracht mit Elektroautos.

LI-Batterien sind leider auch bekannt dafür, dass die Herstellung oft schädlich ist für Mensch und Natur. Deshalb schauen wir drauf, ob man in Zukunft aus der Ressource nicht mehr draus machen kann.

Was die Lebenszeit angeht, gehen die Angaben stark auseinander, zwischen 2 und 10 Jahren und 500-6000 Ladungen findet man einige Zahlen.

Was die Wiederverwendung angeht, werden LI-Batterien oft nach ca. 20-30% Kapazitätsverlust ausgetauscht.
Dann gibt es 2 Möglichkeiten:

1. Wiederaufbereitung zu 40% der Produktionskosten: nochmal am selben Einsatzort einsetzen. Heute sogar zu fast 100% der Leistung
2. Repurposing: Wiederverwendung an einem anderen Einsatzort und -zweck.
  Aus der Ressource wird letztendlich bloß noch mehr Wirtschaftsleistung gepresst. 

 -->

---

**Beispiel:** [PYLONTECH LiFePO4 Speicher 48V - 3,5kWh - US3000 C](https://greenakku.de/Batterien/Lithium-Batterien/48V-Lithium/PYLONTECH-LiFePO4-Speicher-48V-3-5kWh-US3000-C::1968.html?cq_src=google_ads&cq_cmp=19743368784&cq_con=&cq_term=&cq_med=pla&cq_plac=&cq_net=x&cq_pos=&cq_plt=gp&gad_source=1&gclid=Cj0KCQiA1rSsBhDHARIsANB4EJbcofjcW04gEaHBMIy2G2lUqBTGA6U-zwx9_wdNEFs3fF4dPTnSancaAhD7EALw_wcB)

<!-- 
Beispiel für Lithium-Eisenphosphat-Batterie

- 3,3kWh -> Leistung von BS 3kW
- Konsumentenverfügar
- Aneinanderketten für mehrere Batterien ohne Tiefenentladung oder Wechselausfälle

ca. 1000 €
 -->

---

## Leistungsdichte aktueller Batterien
|       | Lithium-Eisenphosphat-Batterien | Lithium-Schwefel-Batterien | Natrium-Ionen-Batterien |
| :---: | :-----------------------------: | :------------------------: | :---------------------: |
| Wh/kg |             200-300             |            300             |         140-160         |
| Wh/l  |             600-750             |            450             |         250-300         |


<!-- _footer: '"Muss es Lithium sein?", c´t 2023, Heft 26, Heise Medien, ISSN 0724-8679' -->

<!-- 
Alternativen für LiFePO4-Batterien:

1. Lithium-Schwefel-Batterien: gut, aber nicht so physisch dicht, wie LiFePO4, Herstellungsprobleme immernoch vorhanden, gerade im Kommen
2. Natrium-Ionen-Batterien: nicht ganz so gut, aber Herstellungsprobleme sind behoben, von umweltbewussten Unternehmen eingesetzt und es wird aktive Forschung betrieben

 -->
---

## Stromverbrauch von gNB Base Stations
*Energieverbrauch und Erneuerbare Energien*

- 240/400-Volt-Stromanschluss (3 kW)

- 14 200 Standorte mit > 43 000 Antennen
- \>50% der Mobilfunkstationen haben 5G-Technologien

:arrow_right: $50\% * 14 200 \space \textrm{Standorte} * 3\frac{kW}{\textrm{Standort}} = 21,3 MW$

:arrow_right: $650 \frac{Wh}{l} / 3 kW = 13 \frac{\textrm{min}}{l}; \quad 250 \frac{Wh}{k} / 3 kW = 5 \frac{\textrm{min}}{kg}$

<!-- _footer: '["Ausbau des 5G-Netzes schreitet weiter voran. 5G jetzt für 90% der Bevölkerung", Newsroom Vodafone, 20.08.2023, https://newsroom.vodafone.de/netz/mobilfunk-netzausbau-5g-netz-fur-90-prozent-der-bevolkerung](https://newsroom.vodafone.de/netz/mobilfunk-netzausbau-5g-netz-fur-90-prozent-der-bevolkerung)' -->

<!-- 
Strom in den Batterien -> Stromverbrauch einer gNB Basis Station
Indikatoren: Energieverbrauch und Erneuerbare Energien

- 1 240/400V-Anschluss, Leistung von 3kW
- in DE 14 200 Standorte mit über 43 000 Antennen
- über 50% davon mit 5G Ausstattung

[Hinweis auf 50%, SA und NSA NR und minimum 3kW]

[Rechnung 50% der Standorte]

[Rechnung auf ungewöhnliche Maße, aber gut für physische Größe und Masse und Verbrauch]

-> Mehr ist mehr
-->

---

## Erneuerbare Stromerzeugung in Deutschland
![h:400 center](bilder/bruttostromerzeugung-erneuerbare-energien.png)
<!-- _footer: '["Bruttostromerzeugung 2022", Statistisches Bundesamt (Destatis), https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Energie/_Grafik/_Interaktiv/bruttostromerzeugung-erneuerbare-energien.html](https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Energie/_Grafik/_Interaktiv/bruttostromerzeugung-erneuerbare-energien.html)' -->

**Veraltet!** Bruttostromerzeugung im [1. Halbjahr 2023](https://www.destatis.de/DE/Presse/Pressemitteilungen/2023/09/PD23_351_43312.html) und [3. Quartal 2023](https://www.destatis.de/DE/Presse/Pressemitteilungen/2023/12/PD23_462_43312.html)

<!-- 
Nutzung von erneuerbaren Energien hängt von der Stromerzeugung ab.

In DE in 2022 44% erneuerbare Energien, generell Windkraft deutlich mehr als Solarenergie oder Wasserkraft.

[neue Zahlen auf der Webseite angucken]

[Hinweis: In idealen Bedingungen generiert ein Solarpanel etwa 1000 Watt pro Quadratmeter Leistung]
[Hinweis: Solar und Wind nicht genutzt, weil die Batterien nicht so lange laufen können und BS verlässlich sein müssen]
-->


---
# 2. Wie stark ist der Einfluss von Mobilkommunikation auf die Umwelt?

- Mobilfunkabdeckung von 89% im Juli 2023
- 14200 Standorte mit mehr als 43000 Antennen
- Jeder Standort á 3kW -> 42,6 MW -> ca. 373 GWh pro Jahr
- von zwischen ca. 500 und 552 TWh Stromverbrauch in DE in 2022
- rund 510 TWh inländisch erzeugt in Deutschland
- bis 2030 sollen 80% erneuerbare Energie sein, insb. Windkraft

<!-- 
Viel gelernt über die Stromerzeugung und Nutzung im Bereich Mobilkommunikation.

Vergleich der Nutzung und Einordnung in Deutschland
- Effizienz: 89% 5G-Abdeckung
- Standortrechnung ohne 50%
- 373,176 GWh pro Jahr
  
neue Infos:
- in DE zwischen 500-552 TWh in einem Jahr verbraucht
- davon 510 TWh inländisch erzeugt
- Politik: bis 2030 sollen 80% erneuerbar sein
-->

---

## Stromverbrauch zusammengefasst

<!-- TODO: wie viel Batterie ist in einer Basisstation? Wie lange kann Strom ausfallen? -->

- bei Betrieb dauerhaft 42,6 MW in Deutschland
- 13 Minuten / Liter verkraftbarer Stromausfall
- ca. **0,071% des Gesamtverbrauchs** in Deutschland gehen auf Basis Stationen zurück

<!-- 
Zusammengefasste Anforderungen

- dauerhaft 43 MW irgendwo herbekommen
- Überbrückung durch Batterien ist eingeschränkt durch Produktions- und Herstellungskosten
- Zahl zum Mitnehmen 0,071% des Gesamtverbrauchs in Deutschland sind Base Stations
-->

---

<!-- 
_class: centered
-->

## Was heißt das für uns?

![h:300 center](https://media.licdn.com/dms/image/C5612AQFoIvbgA_brMw/article-cover_image-shrink_423_752/0/1621725087228?e=1709164800&v=beta&t=3BrtyZypIwxxvJ9SHlnswejemY00yO16gIlaJ6LjJFk)

Hier fehlen verlässliche Zahlen der Branche, Energieverbrauch des User Equipments und Effizienzrechnung $\frac{\textrm{Transmit Power}}{\textrm{Power Consumption}}$

<!-- 
Was heißt das für uns?

Keine Ahnung! So weit bin ich noch nicht

Hier fehlen verlässliche, also einheitliche Zahlen, UE, und Trasmit-Power/Power-Consumption
-->

---

# 3. Wo kommt der Energieverbrauch her?​

**Teile einer Base Station (4G):**
1. Antennensystem
2. RRU (Remote Radio Unit)
3. BBU (Baseband Unit)
4. Physical support (Stromversorgungssystem, Backup-Batterieen, transmittion equipment, air conditioning)

In 5G: RRU und Antennensysteme sind Active Antenna Units (AAU) und BBUs sind Centralized Units (CU) und Distributed (DU).

<!-- _footer: '["What is Base Station?", IPLOOK, 2023, https://www.iplook.com/info/what-is-base-station-i00169i1.html](https://www.iplook.com/info/what-is-base-station-i00169i1.html)' -->

<!-- 
Stattdessen können wir uns darüber unterhalten, aus welchen Bauteilen eine Base Station besteht:

1. Antennensystem: für Laien und uns verständlich
2. RRU (Remote Radio Unit): 
3. BBU (Baseband Unit): 
-->

---

<!-- _class: tableCenter -->

## Energieverbrauch pro Bauteil (circa)

|                            | volle Leistung | Idle     | Deep Sleep |
| -------------------------- | -------------- | -------- | ---------- |
| Active Antenna Units (AAU) | 1130-1180W     | 635-665W | 150-200W   |
| Baseband Units (BBU)       | 295-325W       | 295-320W | 150-320W   |
| Air Conditioning           | 1740W          | 1740W    | 1740W      |

<!-- _footer: '["Remake Green 5G, Mobile Innovation for Climate Action", China Telecom and ZTE, https://www.zte.com.cn/content/dam/zte-site/res-www-zte-com-cn/white_paper/Remake_Green_5G.pdf](https://www.zte.com.cn/content/dam/zte-site/res-www-zte-com-cn/white_paper/Remake_Green_5G.pdf)' -->

---

![h:500 center](bilder/EnergyConsumptionOf5GEquipment.png)

<!-- _footer: '["Remake Green 5G, Mobile Innovation for Climate Action", China Telecom and ZTE, https://www.zte.com.cn/content/dam/zte-site/res-www-zte-com-cn/white_paper/Remake_Green_5G.pdf](https://www.zte.com.cn/content/dam/zte-site/res-www-zte-com-cn/white_paper/Remake_Green_5G.pdf)' -->

---

# 4. Wie kann eingespart werden?​

1. Sidelink enhancements
2. Giga-MIMO
3. NR-Light
4. Lower Transmit Power for IoT devices (Reduced Capability NR)
5. Sleep Modes

---

## NR Sidelink

- basiert auf LTE Sidelink
- Device-to-Device (D2D) Kommunikation
- Distributed Networking - "Distributed Base Stations"

<!-- _footer: '["How will sidelink bring a new level of 5G versatility?", Qualcomm, 08.09.2022, https://www.qualcomm.com/news/onq/2022/09/how-will-sidelink-bring-a-new-level-of-5g-versatility](https://www.qualcomm.com/news/onq/2022/09/how-will-sidelink-bring-a-new-level-of-5g-versatility)' -->

---

![center](https://s7d1.scene7.com/is/image/dmqualcommprod/Picture3-2?$QC_Responsive$&fmt=png-alpha&wid=640)

<!-- _footer: '["How will sidelink bring a new level of 5G versatility?", Qualcomm, 08.09.2022, https://www.qualcomm.com/news/onq/2022/09/how-will-sidelink-bring-a-new-level-of-5g-versatility](https://www.qualcomm.com/news/onq/2022/09/how-will-sidelink-bring-a-new-level-of-5g-versatility)' -->

---

### Verbesserungen durch NR Sidelink

- Erhöhte (Sidelink-)Reichweite
- Vergrößerte Kapazität
- Data Offload

<!-- _footer: '["How will sidelink bring a new level of 5G versatility?", Qualcomm, 08.09.2022, https://www.qualcomm.com/news/onq/2022/09/how-will-sidelink-bring-a-new-level-of-5g-versatility](https://www.qualcomm.com/news/onq/2022/09/how-will-sidelink-bring-a-new-level-of-5g-versatility)' -->

---

##  Giga MIMO

- Vergrößerte Kapazität
- Verbesserter Throughput
- Längere Batterielebenszeit

<hr>

*pot. weitere Verbesserungen in 6G*

---

##  NR-Light

- Geringere Kapazität
- Geringere Komplexität <small style="color: grey;">(150Mbps DL / 50 Mbps UL, 13-30ms latency)</small>
- Geringerer Stromverbrauch

---

##  Reduced Capability (RedCap) NR

![h:450 center](https://www.ericsson.com/cdn-cgi/image/format=auto,fit=scale-down,width=1440/491c72/assets/global/qbank/2021/02/16/redcap-table-2_grey-1287614e7eeaaed91a08c2fa13b5f81d38ad5f.jpg)

<!-- 
FDD: Frequency Division Duplex
TDD: Time Division Duplex
 -->

<!-- _footer: '["What is reduced capability (RedCap) NR and what will it achieve?", Ericsson, 11.02.2021, https://www.ericsson.com/en/blog/2021/2/reduced-cap-nr](https://www.ericsson.com/en/blog/2021/2/reduced-cap-nr)' -->

---

##  Reduced Capability (RedCap) NR

![h:450 center](https://www.ericsson.com/cdn-cgi/image/format=auto,fit=scale-down,width=1440/4911c1/assets/global/qbank/2021/02/11/illustration-of-the-difference-1286077012acc7855968aca64357cb774bc6e6.jpg)

<!-- _footer: '["What is reduced capability (RedCap) NR and what will it achieve?", Ericsson, 11.02.2021, https://www.ericsson.com/en/blog/2021/2/reduced-cap-nr](https://www.ericsson.com/en/blog/2021/2/reduced-cap-nr)' -->

---

##  Reduced Capability (RedCap) NR

- Geringere Bandbreite (20-100 MHz)
- Geringere Anzahl an Receive Antennen
- Kleinere Konstellationsmatrizen für Modulierung
- Optionaler Duplex

<!-- _footer: '["What is reduced capability (RedCap) NR and what will it achieve?", Ericsson, 11.02.2021, https://www.ericsson.com/en/blog/2021/2/reduced-cap-nr](https://www.ericsson.com/en/blog/2021/2/reduced-cap-nr)' -->

---

## Sleep Modes

![h:500 center](bilder/SleepModeSwitching.png)
<!-- _footer: Dynamic gNodeB Sleep Control for Energy-Conserving 5G Radio Access Network; Pengfei Shen et al., 13.07.2022 -->

---

## Sleep Modes

![h:500 center](bilder/SleepModesTransitions.png)
<!-- _footer: Dynamic gNodeB Sleep Control for Energy-Conserving 5G Radio Access Network; Pengfei Shen et al., 13.07.2022 -->

---

### Täglicher Traffic

![h:500 center](bilder/CommTraffic.png)
<!-- _footer: Energy consumption optimization of 5G base stations considering variable threshold sleep mechanism; Xiaoyan Ma et al. -->

---

## Sleep Modes

![h:500 center](bilder/CommTrafficSleep.png)
<!-- _footer: Energy consumption optimization of 5G base stations considering variable threshold sleep mechanism; Xiaoyan Ma et al. -->
<!--
ECOS: Energy Consumption Optimization of 5G BSs
IMAP: Initial Matching Association Process
FTSS: Fixed threshold sleep strategy
MTRS: Maximum transmission rate user association strategy
-->

---
<!-- 
_header: ''
_paginate: skip
-->

![h:600 center](https://media.makeameme.org/created/noch-fragen-e5ff492912.jpg)

---

<!-- _class: tableCenter smalltable -->

# Abkürzungsverzeichnis

| Abkürzung | Bedeutung                                           |
| --------- | --------------------------------------------------- |
| NR        | New Radio (5G)                                      |
| FDD       | Frequency Division Duplex                           |
| TDD       | Time Division Duplex                                |
| ECOS      | Energy Consumption Optimization of 5G BSs           |
| IMAP      | Initial Matching Association Process                |
| FTSS      | Fixed threshold sleep strategy                      |
| MTRS      | Maximum transmission rate user association strategy |

---

<!-- _class: centered
 -->

# Presenter
![](https://media.licdn.com/dms/image/C5603AQGSV-yyfbgmeg/profile-displayphoto-shrink_200_200/0/1623311887654?e=1709769600&v=beta&t=qPack9A-o02XTnsWjvev62PBJEjEiMXSUscabd7qR_o)
Andreas Nicklaus

<div style="display: flex; justify-content: space-around;">
  <div>
    <a href="https://www.instagram.com/andreasnicklaus">
      <img src="https://upload.wikimedia.org/wikipedia/commons/9/96/Instagram.svg" height="60">
      <br>
      @andreasnicklaus
    </a>
  </div>
  <div>
    <a href="https://www.linkedin.com/in/andreasnicklaus/">
      <img src="https://upload.wikimedia.org/wikipedia/commons/8/81/LinkedIn_icon.svg" height="60">
      <br>
      andreasnicklaus
    </a>
  </div>
  <div>
    <a href="https://www.www.andreasnicklaus.de">
      <img src="https://img.icons8.com/ios/100/000000/domain--v1.png" height="60">
      <br>
      andreasnicklaus.de
    </a>
  </div>
</div>