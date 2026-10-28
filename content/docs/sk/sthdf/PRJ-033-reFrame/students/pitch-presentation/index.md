---
# Versioning – systém dopĺňa automaticky
fm_version: "1.0.1"

# Dátum buildu – generuje skript
fm_build: "2026-10-28T11:40:00+00:00"

# Poznámka k verzii – voliteľné
fm_version_comment: "Scenár a slajdy Pitch prezentácie pre Re:Frame 35"


# IDENTITY --------------------------------------------------------

# ID generuje CLI / skript
id: "PRJ-033-reFrame-pitch-presentation"

# Unikátne UUID – generuje skript
guid: "f81447f3-7ba6-4907-9216-48d3639d136c"


# CONTEXT ---------------------------------------------------------

# DAO / doména (knife, sdlc, q12, 7ds...) dopĺňa skript
dao: "sthdf"

# Názov zápisu – dopĺňa používateľ
title: "Pitch Presentation – Re:Frame 35"

# Krátky popis – dopĺňa používateľ (voliteľné)
description: "Prezentačný koncept a scenár krátkeho 3–5 minútového pitchu projektu Re:Frame 35."


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
type: "pitch-presentation"

# Priorita (low/medium/high) – voliteľné
priority: "medium"

# Tagy – odporúča sa 2–6 tagov.
tags:
  - "sthdf"
  - "pitch"
  - "presentation"
  - "reframe35"


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

# Pitch Presentation (Re:Frame 35)

## 1. Problém
- **Digitálne dáta sú krehké:** Expirované WeTransfer odkazy z fotolabov alebo poškodené SSD disky, zrušené cloudové kontá spôsobujú trvalú stratu fotografií.
- **Fyzický negatív prežije 100 rokov:** Doma máme uložený najodolnejší offline archív (*cold storage*), no nemáme ho ako pohodlne a bezplatne vyvolať.
- **Bariéry komerčnej digitalizácie:** Ploché skenery na filmy stoja viac ako 300 €, dedikované softvérové pluginy vyžadujú drahé predplatné a komerčný resken v laboratóriu stojí 8 až 12€ za jeden film.

---

## 2. Riešenie: Re:Frame 35
- **Prepojenie 3D tlače a počítačového videnia:**  
  Systém pozostávajúci z 3D tlačenej optickej komory s rovnomerným LED podsvietením a sprievodného Python algoritmu (OpenCV).
- **Využitie smartfónu:**  
  Namiesto nákupu nového drahého skenera využívame snímač a optiku, ktorú už každý nosí vo vrecku.

---

## 3. Hodnota
- **Nulové priebežné náklady:** Digitalizácia celého 36-obrázkového filmu stojí len pár centov elektrickej energie.
- **Rýchlosť:** Digitalizácia a softvérový prevod jedného políčka trvá len sekundy, celý film je hotový do 10 minút.
- **Bezpečnosť média:** Premyslená konštrukcia s bezdotykovou zónou zabezpečuje, že emulzia filmu neprichádza do styku s mechanickými časťami a nehrozí jej poškriabanie.
- **Vysoké rozlíšenie:** Moderné snímače smartfónov poskytujú dostatočné rozlíšenie na tlač veľkých formátov.

---

## 4. Biznis model
- **Open-source:** 3D modely (`.STL`) a Python kód sú voľne dostupné pre komunitu (MIT / CC-BY licencia).

---

## 5. Tím
- **ST014 (Milan Šeliga):** Co-Lead (Software / CV) – architektúra OpenCV pipelineu, normalizácia oranžovej masky, projektová integrácia.
- **ST016 (Margaréta Strýčková):** Co-Lead (Hardware / CAD) – CAD návrh optického tubusu, optimalizácia tolerancií tlače, návrh svetelnej difúzie.

---

## 6. Call to action
- **Čo hľadáme:** Spätnú väzbu na kvalitu tonálneho prevodu od skúsenejších fotografov poprípade dobrovoľníkov na otestovanie rôznych modelov smartfónov (iOS / Android) a filmových emulzií (Kodak, Fujifilm, ...).

---
<!-- 
## Štruktúra pitchu
Prezentácia (cca 3–4 minúty) pokrýva 5 hlavných tém:
1. **Problém** – drahá a nepraktická digitalizácia kinofilmov v domácich podmienkach.
2. **Riešenie** – Re:Frame 35 (spojenie 3D tlačenej komory, smartfónu a Python algoritmu).
3. **Prínos a hodnota** – rýchly prevod do 10 minút, nulové priebežné náklady a šetrnosť k filmu.
4. **Rozdelenie úloh v tíme** – softvér a spracovanie obrazu (Milan) vs. hardvér a konštrukcia (Margaréta).
5. **Výzva a ďalšie kroky** – testovanie rôznych typov filmov a zber spätnej väzby. -->

---

## Navigácia
- [Späť](../index.md)
