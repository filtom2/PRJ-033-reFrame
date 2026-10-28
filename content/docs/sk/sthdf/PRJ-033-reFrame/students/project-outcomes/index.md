---
# Versioning – systém dopĺňa automaticky
fm_version: "1.0.1"

# Dátum buildu – generuje skript
fm_build: "2026-10-28T11:40:00+00:00"

# Poznámka k verzii – voliteľné
fm_version_comment: "Výstupy projektu Re:Frame 35 podľa SDLC a V-modelu"


# IDENTITY --------------------------------------------------------

# ID generuje CLI / skript
id: "PRJ-033-reFrame-project-outcomes"

# Unikátne UUID – generuje skript
guid: "d91e5e9d-6ab6-422e-b662-b0d76a2f8df0"


# CONTEXT ---------------------------------------------------------

# DAO / doména (knife, sdlc, q12, 7ds...) dopĺňa skript
dao: "sthdf"

# Názov zápisu – dopĺňa používateľ
title: "Project Outcomes – Re:Frame 35"

# Krátky popis – dopĺňa používateľ (voliteľné)
description: "Prehľad dosiahnutých výsledkov, technických artefaktov (CAD, Python) a overenia systému Re:Frame 35."


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
type: "project-outcomes"

# Priorita (low/medium/high) – voliteľné
priority: "high"

# Tagy – odporúča sa 2–6 tagov.
tags:
  - "sthdf"
  - "project-outcomes"
  - "sdlc"
  - "cad"
  - "python"
  - "mvp"


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

# Project Outcomes

## Stav projektu
- **Aktuálny stav:** Dizajnová fáza
- **Čo je pripravené (dizajn a koncept):**
  - CAD modely jednotlivých častí optickej komory (základňa, drážka s bezdotykovou zónou pre emulziu, optický tubus).
  - Konceptuálny návrh Python algoritmu pre odčítanie oranžovej masky C-41 a tonálnu transformáciu.
- **Čo nás čaká (nasledujúce kroky):**
  - Prvá testovacia 3D tlač mechanických dielov a overenie rozmerových tolerancií posuvu filmu.
  - Zostavenie komory s LED podsvietením a difúznymi sklami.
  - Praktická implementácia a ladenie Python skriptu na reálnych fotkách negatívov zhotovených v komore.

---

## Výstupy podľa SDLC / V-modelu

### 1. Business požiadavky
- Vytvorenie nezávislého, cenovo dostupného systému na obnovu a archiváciu fotografií z vyvolaných kinofilmov v domácich podmienkach (celková cena hardvéru pod 15 €).
- Odstránenie nutnosti platiť drahé komerčné skeny (8–12 € / film).

### 2. Top Level Architecture
- **Hardvérová úroveň:** Stolný optický tubus s LED svetelným zdrojom, difúznou komorou, filmovým slotom a držiakom telefónu.
- **Softvérová úroveň:** Lokálny spracovateľský skript v Pythone komunikujúci s lokálnym súborovým systémom (vstup: nasnímaný negatív, výstup: rekonštruovaný pozitív).

### 3. Solution Architecture
- **Fyzická integrácia:** Modulárny skladací systém (základňa, svetelná komora, vodiaci tunel, zvislý tubus, adaptér mobilu).
- **Algoritmická štruktúra:**
  1. Predspracovanie a prevod do `float32`.
  2. Segmentácia neexponovanej bázy filmu pre odčítanie masky.
  3. Farebná separácia a lineárna normalizácia kanálov.
  4. Inverzia do pozitívu a automatické vyváženie bielej (Percentile / Gray-World).
  5. Nelineárna kontrastná transformácia (S-curve).

### 4. Analysis
- Detailný rozbor rozmerov kinofilmu podľa **ISO 1007** (šírka pásu $35\text{ mm}$, výška obrazového poľa $24\text{ mm}$, šírka poľa $36\text{ mm}$, rozteč perforácií $4.75\text{ mm}$).
- Optická analýza minimálnej zaostrovacej vzdialenosti moderných smartfónov (ohnisková vzdialenosť vyžaduje tubus výšky $110 - 140\text{ mm}$ pri použití štandardného 1× širokouhlého objektívu).

### 5. Design (Aktuálna fáza)
- CAD návrh komponentov v `.STEP` a `.STL` formáte (Margaréta).
- Optimalizácia tlačových vrstiev (orientácia tlače bez nutnosti podporných štruktúr pre hladký chod filmu).
- Návrh rozmerov a tolerancií vodiacej drážky (35.25 mm) s bezdotykovou zónou pre emulziu.

### 6. Implementation (Plánované)
- Výroba dielov na 3D tlačiarni z materiálov Matte Black PLA (tubus) a PETG (základňa a mechanické spoje).
- Implementácia skriptu `process_film.py` a súboru `requirements.txt`.

### 7. Verification & Testing (Plánované)
- **Mechanické testovanie:** Overenie hladkého posuvu filmu v drážke bez rizika vzniku mikroškrabancov na obrazovom poli.
- **Optické testovanie:** Meranie rovnomernosti podsvietenia a difúzie v snímanom poli $24 \times 36\text{ mm}$.
- **Algoritmické testovanie:** Testovanie farebnej rekonštrukcie na rôznych typoch filmov (Kodak ColorPlus, Kodak Gold, Fujifilm Superia).

### 8. Operation (Plánované)
- Používateľ položí telefón na hornú platformu, zasunie film, odfotí políčko a skript automaticky spracuje a uloží výslednú fotografiu.

---

## Finálny produkt (Plánované výstupy)

### 1. Hardvérový balík (CAD modely & BOM)
Pripravené CAD súbory na následný slicing a 3D tlač:
- `ReFrame35_Base.stl` – základňa s uchytením LED panela
- `ReFrame35_DiffuserTray.stl` – slot na akrylový difúzor ($45 \times 60\text{ mm}$)
- `ReFrame35_FilmGuide.stl` – vodiaca drážka s $0.5\text{ mm}$ emulzným odskokom
- `ReFrame35_OpticalCone.stl` – svetlotesný zvislý tubus
- `ReFrame35_PhoneAdapter.stl` – vrchná kolíska telefónu

#### Kusovník plánovaného materiálu (BOM – Bill of Materials)
| Komponent | Špecifikácia | Množstvo | Odhadovaná cena |
|:---|:---|:---:|:---:|
| Filament PLA (Matte Black) | 3D tlač tela a tubusu (cca 180 g) | 1 ks | 4.50 € |
| LED svetelný modul | 5V USB LED panel, High CRI $\ge 95$ | 1 ks | 5.20 € |
| Opálové akrylové sklo | Difúzor 2mm, priepustnosť 70 % | 2 ks | 2.50 € |
| Spojovací materiál | Skrutky M3 × 12mm a mosadzné vložky | 6 ks | 1.20 € |
| **Spolu** | | | **13.40 €** |

### 2. Softvérový balík (Plánovaná implementácia)
- `process_film.py` – skript pre dávkovú aj individuálnu konverziu negatívov.
- Závislosti: `opencv-python`, `numpy`, `matplotlib`.

- **Odkaz na repozitár:** [https://github.com/filtom2/PRJ-033-reFrame](https://github.com/filtom2/PRJ-033-reFrame)

---

## Porovnanie s Project Summary

| Parameter / Cieľ | Plán v Project Summary | Aktuálny stav (Dizajnová fáza) | Stav plnenia |
|:---|:---|:---|:---:|
| **Hardvérový prototyp** | Funkčná 3D optická komora s LED | Dokončený CAD dizajn dielov, čaká na prvú 3D tlač | V procese |
| **Spracovateľský kód** | Automatizovaný Python skript (OpenCV) | Navrhnutá architektúra a postup spracovania C-41 | V procese |
| **Rozpočet (BOM)** | Náklady pod 15 € | Predbežný kusovník materiálu na úrovni 13.40 € | V pláne |
| **Otestovanie na filmoch** | Overenie na reálnych filmoch | Pripravené vzorky kinofilmov na následné testy | V pláne |

---

## Navigácia
- [Späť](../index.md)
