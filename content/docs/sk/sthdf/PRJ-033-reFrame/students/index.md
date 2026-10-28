---
# Versioning – systém dopĺňa automaticky
fm_version: "1.0.1"

# Dátum buildu – generuje skript
fm_build: "2026-10-28T11:40:00+00:00"

# Poznámka k verzii – voliteľné
fm_version_comment: "Aktualizovaný rozcestník študentských výstupov pre Re:Frame 35"


# IDENTITY --------------------------------------------------------

# ID generuje CLI / skript
id: "PRJ-033-reFrame-students"

# Unikátne UUID – generuje skript
guid: "79f47ded-ea82-4ae1-8376-33c0edf118b9"


# CONTEXT ---------------------------------------------------------

# DAO / doména (knife, sdlc, q12, 7ds...) dopĺňa skript
dao: "sthdf"

# Názov zápisu – dopĺňa používateľ
title: "Študentské deliverables – Re:Frame 35"

# Krátky popis – dopĺňa používateľ (voliteľné)
description: "Rozcestník a kontrolný checklist 7 povinných výstupov projektu Re:Frame 35 (ST014 & ST016)."


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
type: "students-hub"

# Priorita (low/medium/high) – voliteľné
priority: "high"

# Tagy – odporúča sa 2–6 tagov.
tags:
  - "sthdf"
  - "deliverables"
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

# Moje deliverables (Re:Frame 35)

Toto je rozcestník k povinným výstupom študentského tímu pre predmet **Systémové myslenie v IT a digitálna fabrikácia (SMVIT / STHDF)**.

## Navigácia v sekciách
- [01 – About Us (Autorská dvojica)](./about-me/index.md)
- [02 – Knowledge Contribution (KNIFE)](./knowledge-contribution/index.md)
- [03 – Project Summary](./project-summary/index.md)
- [04 – Project Outcomes](./project-outcomes/index.md)
- [05 – Pitch Presentation](./pitch-presentation/index.md)
- [06 – Final Presentation](./final-presentation/index.md)
- [07 – Reflexia](./reflexia/index.md)

> Poznámka k **Knowledge Contribution**: toto deliverable je v systéme reprezentované ako **KNIFE** (odborný technický článok so špecifickým zameraním na algoritmickú kompenzáciu C-41 farebného kinofilmu v OpenCV).

## Rýchly checklist
- [x] **About Us (Autorská dvojica)** vyplnené (profily, deľba práce, kontakty)
- [ ] **Knowledge Contribution (KNIFE)** v príprave
- [x] **Project Summary** vyplnené (kompletný projektový zámer od identifikácie po riziká)
- [x] **Project Outcomes** pripravené (BOM rozpočet pod 15 €, CAD zostava, Python pipeline)
- [x] **Pitch Presentation** hotová (5 slajdov na 3–5 minútový pitch)
- [ ] **Final Presentation** v príprave
- [ ] **Reflexia** v príprave

## Ako pracovať (mini-návod)
1. Otvor príslušnú stránku vyššie a doplň alebo skontroluj obsah.
2. Skontroluj odkazy na repozitár, video a demo podklady.
3. Ulož zmeny, commitni a pushni:
   ```bash
   git add .
   git commit -m "Update deliverables: complete 7 sections for Re:Frame 35"
   git push
   ```

## Navigácia
- [Späť](../../index.md)
