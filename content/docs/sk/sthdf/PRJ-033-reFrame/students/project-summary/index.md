---
# Versioning – systém dopĺňa automaticky
fm_version: "1.0.1"

# Dátum buildu – generuje skript
fm_build: "2026-10-28T11:40:00+00:00"

# Poznámka k verzii – voliteľné
fm_version_comment: "Kompletné vyplnenie Project Summary pre Re:Frame 35"


# IDENTITY --------------------------------------------------------

# ID generuje CLI / skript
id: "PRJ-033-reFrame-project-summary"

# Unikátne UUID – generuje skript
guid: "d0441cfd-35d4-4767-80d8-e1938142fc7e"


# CONTEXT ---------------------------------------------------------

# DAO / doména (knife, sdlc, q12, 7ds...) dopĺňa skript
dao: "sthdf"

# Názov zápisu – dopĺňa používateľ
title: "Project Summary – Re:Frame 35"

# Krátky popis – dopĺňa používateľ (voliteľné)
description: "Detailné projektové zhrnutie nízkonákladového poloautomatického systému na obnovu fotografií z 35mm kinofilmu Re:Frame 35."


# AUTHORSHIP ------------------------------------------------------

# Autori projektu – rovnocenná autorská dvojica
author: "Milan Šeliga & Margaréta Strýčková"

# Zoznam autorov – generuje skript
authors:
  - "Milan Šeliga (ST014)"
  - "Margaréta Strýčková (ST016)"


# CLASSIFICATION ---------------------------------------------------

# Nadradená kategória – môže doplniť používateľ
category: "STHDF"

# Typ dokumentu (guide, case, tutorial...) – používateľ (voliteľné)
type: "project-summary"

# Priorita (low/medium/high) – voliteľné
priority: "high"

# Tagy – odporúča sa 2–6 tagov.
tags:
  - "sthdf"
  - "computer-vision"
  - "3d-printing"
  - "c41"
  - "hardware"
  - "python"


# LOCALIZATION -----------------------------------------------------

# Jazyk dokumentu – doplní skript podľa štruktúry
locale: "sk"


# LIFECYCLE --------------------------------------------------------

# Dátum vytvorenia – generuje skript
created: "2026-10-28"

# Dátum poslednej úpravy – dopĺňa človek
modified: "2026-10-28"

# Stav dokumentu – default "backlog"
status: "active"

# Viditeľnosť – default "public"
privacy: "public"


# INTELLECTUAL PROPERTY -------------------------------------------

# Držiteľ práv k obsahu – dopĺňa skript
rights_holder_content: "Milan Šeliga, Margaréta Strýčková (FIIT STU)"

# Systémový vlastník práv
rights_holder_system: "CAA / KNIFE / LetItGrow"

# Licencia
license: "CC-BY-NC-SA-4.0"

# Disclaimer
disclaimer: "Use at your own risk. Methods provided as-is; participation is voluntary and context-aware."

# Copyright
copyright: "© 2026 Milan Šeliga, Margaréta Strýčková"


# ORIGIN / PROVENANCE ---------------------------------------------

# Repozitár pôvodu
origin_repo: "https://github.com/filtom2/PRJ-033-reFrame"

# URL pôvodného repozitára
origin_repo_url: "https://github.com/filtom2/PRJ-033-reFrame"

# Commit pôvodu
origin_commit: ""

# Branch pôvodu
origin_branch: "main"

# Systém pôvodu (CAA/KNIFE/STHDF…)
origin_system: "CAA"

# Pôvodní autori
origin_author: "Milan Šeliga & Margaréta Strýčková"

# Importovaný zdroj
origin_imported_from: ""

# Dátum importu
origin_import_date: ""


# RESERVED ---------------------------------------------------------

fm_reserved1: ""
fm_reserved2: ""
---

<!-- SDLC_INSTANCE_ID: PRJ-033-reFrame -->

# Project Summary

## Identifikácia

### 1. Názov projektu
- **Kód a názov projektu:** `PRJ_033_ReFrame35_ST014_ST016` (skrátený komerčný názov: **Re:Frame 35**)
- **Stručný popis:**  
  Re:Frame 35 je nízkonákladový poloautomatický systém na obnovu fotografií z vyvolaných 35mm filmových negatívov. Spája na mieru navrhnutú 3D tlačenú optickú komoru pre smartfón s algoritmickým pipelineom v Pythone (OpenCV). Zariadenie rieši problém straty digitálnych kópií tým, že pristupuje k fyzickému negatívu ako k trvácnemu offline archívu (*cold storage*), z ktorého dokáže kedykoľvek rýchlo a bezplatne vyextrahovať hotovú digitálnu fotografiu vo vysokej kvalite.

---

### 2. Členovia tímu (Rovnocenná autorská dvojica)

| ST ID | Meno a priezvisko | Rola v tíme | Kompetencie |
|:---|:---|:---|:---|
| **ST014** | **Milan Šeliga** | Rovnocenný autor & Co-Lead (Software / CV) | Koordinácia projektu, návrh a implementácia algoritmov spracovania obrazu (Python/OpenCV), integrácia pipelineu |
| **ST016** | **Margaréta Strýčková** | Rovnocenná autorka & Co-Lead (Hardware / CAD) | Koordinácia projektu, návrh 3D modelov v CAD, ladenie tolerancií aditívnej výroby (FDM), integrácia LED osvetlenia a difúzie |
| **ST014 & ST016** | **Milan Šeliga & Margaréta Strýčková** | QA & Dokumentácia (Spoločne) | Testovanie presnosti orezu a farebnej kalibrácie, technická dokumentácia, príprava testovacieho datasetu |

---

### 3. Motivácia tímu

- **Prečo sme si vybrali tento projekt:**  
  Máme osobný vzťah k analógovej fotografii a zároveň hľadáme praktické prepojenie fyzického prototypovania s počítačovým videním. Fascinuje nás myšlienka vytvoriť reálny, hmatateľný nástroj, ktorý nie je len dekoráciou, ale plnohodnotným pracovným nástrojom.
- **Osobný a profesijný zmysel:**  
  Projekt nám umožňuje prehĺbiť si zručnosti v dvoch kľúčových technických oblastiach: presné mechanické inžinierstvo pre 3D tlač (rešpektovanie mikrometrových tolerancií filmu) a nízkoúrovňové spracovanie obrazu bez použitia hotových proprietárnych „čiernych skriniek“.
- **Prečo je projekt dôležitý a aký problém rieši:**  
  V digitálnom svete čelíme fenoménu straty dát – expirované linky z fotolaboratórií, zlyhania pevných diskov alebo zmazané cloudové úložiská. Mnoho ľudí má doma vyvolané negatívy, ktorých digitálne súbory sa stratili alebo existujú len v zastaranom, nízkom rozlíšení spred 15 rokov. Komerčné reskenovanie je drahé (cca 8–12 € za film) a pomalé. Negatív funguje ako trvácna fyzická záloha a náš projekt k nemu vytvára dostupnú digitálnu čítačku.

---

### 4. Cieľ a pridaná hodnota projektu

- **Finálny cieľ:**  
  Zostaviť funkčný, opakovane použiteľný stolný skener (3D tlačené telo + difúzne LED podsvietenie) a sprievodný softvérový skript, ktorý po vložení negatívu a odfotení smartfónom automaticky narovná perspektívu, odstráni oranžovú masku C-41 a vyexportuje farebne verný pozitív.
- **Ako spoznáme, že je projekt úspešný:**
  1. **Časová metrika:** Digitalizácia a softvérový prevod celého kinofilmu (36 políčok) zaberie menej ako 10 minút.
  2. **Bezpečnosť média:** Vodiaca drážka nepoškriabe emulziu filmu ani po 50 posuvoch (vďaka bezdotykovej zóne).
  3. **Algoritmická autonómia:** Skript dokáže bez manuálneho zásahu korektne vyvážiť bielu a odstrániť oranžovú masku pri minimálne 90 % bežne exponovaných záberov.

---

### 5. Popis riešenia

Riešenie prepája tri základné piliere v jednotnom procesnom toku:

1. **Vstup:** Pás vyvolaného 35mm kinofilmu vložený do vodiaceho slotu.
2. **Fyzická optická komora (3D tlač):**
   - plošné LED podsvietenie s vysokým indexom podania farieb (High CRI),
   - dvojstupňový opálový difúzor na rovnomerné rozptýlenie svetla,
   - vodiaci tunel s ochranným odskokom pre emulziu,
   - svetlotesný tubus s držiakom mobilného telefónu.
3. **Snímanie obrazu:** Surová fotografia (RAW alebo JPG) zachytená mobilným telefónom.
4. **Spracovanie obrazu (Python + OpenCV):**
   - detekcia hrán a rektifikácia rámika políčka,
   - odčítanie oranžovej masky C-41 z referenčnej bázy filmu,
   - normalizácia kanálov a automatické vyváženie bielej,
   - aplikácia tonálnej S-krivky pre filmový kontrast.
5. **Výstup:** Finálna digitálna fotografia (pozitív) pripravená na archiváciu.

- **Čo riešime mechanicky:**  
  Vytvárame kontrolované svetelné prostredie. Odstraňujeme parazitné odlesky z okolia matným vnútorným povrchom tubusu, zabezpečujeme kolmosť optickej osi mobilu voči rovine filmu a fixujeme presnú vzdialenosť zaostrenia (minimálna zaostrovacia vzdialenosť makro/hlavného modulu fotoaparátu).
- **Čo riešime softvérovo:**  
  Riešime chémiu farebného negatívu. Štandardná inverzia farieb ($255 - I$) zlyháva pre prítomnosť oranžovej masky filmu. Náš algoritmus masku matematicky neutralizuje vzorkovaním neexponovanej bázy filmu, normalizuje farebné kanály a nelineárne rozťahuje dynamický rozsah scény.

---

### 6. Projektový plán

- **Odhadovaný čas na prácu:** 4 – 6 hodín / týždeň na jedného člena tímu.
- **Predpokladaný stav v čase záverečnej prezentácie:** Plne funkčné hardvérové MVP (fyzický skener) + otestovaný automatizovaný Python pipeline spracovania.
- **Hlavné míľniky:**
  - [x] **Príprava a rešerš:** Špecifikácia rozmerov 35mm filmu (ISO 1007), optické požiadavky na ohniskovú vzdialenosť telefónu, analýza C-41 chémie.
  - [x] **Dizajnová fáza:** CAD návrh jednotlivých dielov optickej komory (Margaréta), konceptuálny návrh algoritmu na odstránenie masky v Pythone (Milan).
  - [ ] **Výroba prototypu:** 3D tlač dielov na FDM tlačiarni, osadenie LED podsvietenia a difúzora.
  - [ ] **Testovanie a kalibrácia:** Overenie hladkého posuvu filmu v drážke, meranie rovnomernosti difúzie svetla, ladenie tonálnej krivky.
  - [ ] **Finálna prezentácia:** Spracovanie ukážok pred/po, kompletizácia dokumentácie a obhajoba prototypu.

#### Míľniky a výstupy (Do januára dodáme):
- **Prototyp:** Zložená 3D tlačená optická komora s funkčným LED podsvietením a slotom na telefón.
- **Dokumentácia:** Technická správa s parametrami tolerancií tlače, popísaným algoritmom a návodom na obsluhu.
- **Prezentácia:** Slajdy demonštrujúce riešenie problému straty dát, rekonštrukciu fotografií a živé demo skenovania.

---

### 7. Zákazník a hodnoty

- **Kto je používateľom:**
  1. **Analógový fotograf:** Stratil pôvodné digitálne skeny z fotolabu alebo mu expiroval odkaz na stiahnutie (WeTransfer / lab cloud).
  2. **Domáci archivár:** Vlastní rodinné negatívy z 80.–90. rokov a nechce platiť stovky eur za ich komerčnú digitalizáciu.
  3. **Makerspace / študentská komunita:** Hľadá lacný open-source hardvér pre prácu s filmom a experimentovanie s počítačovým videním.
- **Čo mu to prinesie:**
  Nezávislosť od externých komerčných služieb, nulové dodatočné náklady na digitalizáciu, rýchlosť (fotka je pripravená za pár sekúnd) a záchranu rodinných spomienok v modernom vysokom rozlíšení.

---

### 8. Očakávané výstupy

- **Dokumentácia:**
  Prehľadný GitHub repozitár s `README.md` (postup montáže, inštalácia Python balíčkov, príklady volania skriptu), odborný KNIFE článok o princípoch algoritmickej C-41 inverzie.
- **Artefakty:**
  CAD modely (`.STEP` a `.STL` pripravené na slicing), Python CLI skript / modul, vzorová testovacia sada dát (raw skeny negatívov vs. finálne vyvolané fotografie).
- ** Kontext (Literatúra a inšpirácie):**
  - OpenCV Documentation: Image processing, geometric image transformations, contour detection.
  - ISO 1007: Photographic 135-size film and magazine specifications.
  - Princípy farebnej chémie C-41 procesu (odčítanie masky oranžovej bázy filmu).
  - Komunitné open-source 3D projekty filmových adaptérov (Thingiverse, Printables).
- ** Riziká a závislosti:**
  - *Optická rovnorodosť:* Riziko nerovnomerného svetla (hotspoty z LED) $\to$ **Riešenie:** Použitie viacvrstvového opálového difúzora s presným dištančným odstupom od LED čipov.
  - *Geometrické tolerancie 3D tlače:* Riziko trenia filmu v drážke $\to$ **Riešenie:** Pridanie tolerancie $+0.2\text{ mm}$ na šírku a zapustená bezdotyková stredová drážka chrániaca obrazové pole.
  - *Rozmanitosť fotoaparátov mobilov:* Rôzne umiestnenie šošoviek $\to$ **Riešenie:** Modulárny vrchný adaptér, ktorý sa dá vymeniť podľa modelu telefónu bez nutnosti tlačiť celé šasi nanovo.

---

### 9. Reflexia a ďalšie kroky

- **Čo očakávame, že sa naučíme:**  
  Praktické skúsenosti s CAD dizajnom funkčných dielov s ohľadom na FDM technológiu tlače, hlbšie pochopenie farebných priestorov (RGB, LAB, logaritmické krivky) a ladenie algoritmov počítačového videnia na reálnych dátach so šumom.
- **Ako by sa projekt mohol rozvíjať ďalej:**  
  Pridanie krokového motora s prevodom (napr. 28BYJ-48 riadený cez Arduino/ESP32) pre plne automatický motorizovaný posuv filmu; vytvorenie lokálneho webového rozhrania (Streamlit/FastAPI) na interaktívne ladenie farebných kriviek v reálnom čase.

---

## Navigácia
- [Späť](../index.md)
