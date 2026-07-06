# Naturblikk – Arkitektur

> Versjon 0.1

## Mål

Naturblikk skal være en moderne plattform for direktesendt norsk natur.

Løsningen skal være modulær, slik at hver del kan videreutvikles uten å påvirke resten av systemet.

---

# Arkitektur

                    Besøkende
                         │
                         ▼
                https://naturblikk.no
                         │
                  WordPress (CMS)
                         │
         ┌───────────────┼────────────────┐
         │               │                │
         ▼               ▼                ▼
      Live-side       Artikler        Informasjon
         │
         ▼
      Videospiller
         │
         ▼
      MediaMTX
         │
     OBS Studio
         │
 ┌───────┴────────┐
 │                │
 ▼                ▼
Kamera 1      Kamera 2

---

# Delsystemer

## WordPress

Ansvar:

- Forside
- Live-side
- Om-side
- Kontakt
- Nyheter

WordPress skal være CMS – ikke streamingmotor.

---

## Streaming

Består av:

- Tapo C310
- OBS Studio
- MediaMTX

OBS mottar videostrømmer fra kameraene.

OBS kan legge på:

- logo
- klokke
- vær
- tekst
- AI-overlay

Deretter sendes én strøm videre til MediaMTX.

---

## AI

Fase 1

- Fuglegjenkjenning
- Talefiltrering
- Lydanalyse

Fase 2

- Individtelling
- Artsstatistikk
- Automatisk høydepunkt

---

## Backend

Backend skal håndtere:

- API
- Database
- AI-resultater
- Statistikk
- Historikk
- Vær

WordPress skal hente data fra API-et.

---

## Database

Planlagte tabeller

BirdSpecies

BirdObservations

Weather

Events

CameraStatus

Statistics

---

# Modulprinsipp

Alle deler skal kunne byttes ut.

Eksempel:

Tapo

↓

Reolink

↓

PTZ

uten å påvirke nettsiden.

Samme gjelder AI.

---

# Fremtidige lokasjoner

Systemet skal støtte flere lokasjoner.

Eksempel:

Naturblikk

├── Helgeland

├── Vega

├── Lofoten

├── Dovrefjell

└── Hardangervidda

Alle bruker samme backend.

---

# Teknologi

Nettside

- WordPress
- Kadence

Streaming

- OBS
- MediaMTX

AI

- Python

Backend

- Python FastAPI (foreslått)

Database

- SQLite først
- PostgreSQL senere

---

# Designprinsipp

Naturblikk skal være:

- rask
- rolig
- enkel
- moderne
- naturfokusert

Ingen unødvendige animasjoner.

Ingen visuell støy.

Livestreamen skal alltid være hovedfokuset.

---

# Første milepæl

- WordPress
- Live-side
- Ett kamera
- OBS
- Stabil videostrøm

Alt annet kommer etter dette.
