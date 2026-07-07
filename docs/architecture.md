# Naturblikk – Arkitektur

> Versjon 0.2

## Mål

Naturblikk skal starte som et enkelt hobbyprosjekt med WordPress som publiseringsplattform og livestream direkte på forsiden.

Løsningen skal være enkel nå, men strukturert nok til at streaming, AI, statistikk og flere kameraer kan bygges på senere.

---

# Nåværende arkitektur

```text
Besøkende
     │
     ▼
https://naturblikk.no
     │
     ▼
WordPress + Kadence
     │
     ├── Forside med livestream
     ├── Om prosjektet
     ├── Arter
     ├── Galleri
     ├── Kontakt
     └── Personvern
```

I første versjon skal livestreamen ligge på forsiden. En egen Live-side kan vurderes senere hvis prosjektet får flere kameraer eller mer avanserte visninger.

---

# Fremtidig streamingflyt

```text
Tapo C310
     │
     ▼
RTSP
     │
     ▼
OBS Studio
     │
     ▼
MediaMTX
     │
     ▼
Videospiller på naturblikk.no
```

---

# Delsystemer

## WordPress

Ansvar:

- Forside
- Om prosjektet
- Arter
- Galleri
- Kontakt
- Personvern
- SEO
- Annonseplasseringer senere

WordPress skal være nettside og publiseringsplattform – ikke streamingmotor.

---

## Streaming

Består av:

- Tapo C310
- RTSP
- OBS Studio
- MediaMTX

OBS kan etter hvert legge på:

- logo
- klokke
- vær
- tekst
- diskret overlay

Deretter sendes én strøm videre til nettsiden.

---

## AI

AI kommer senere og skal ikke være del av MVP.

Mulige funksjoner:

- Fuglegjenkjenning
- Talefiltrering
- Lydanalyse
- Individtelling
- Artsstatistikk
- Automatisk høydepunkt

---

## Backend

Backend bygges først når det finnes et konkret behov.

Mulige fremtidige ansvarsområder:

- API
- Database
- AI-resultater
- Statistikk
- Historikk
- Værdata

---

# Modulprinsipp

Teknologi kan byttes ut senere uten at hele prosjektet må bygges på nytt.

Eksempler:

```text
Tapo → Reolink → PTZ
```

```text
WordPress → egen frontend
```

Slike bytter er mulige, men skal ikke prioriteres før prosjektet faktisk trenger det.

---

# Teknologi nå

Nettside:

- WordPress
- Kadence Theme
- Kadence Blocks

Streaming:

- OBS
- MediaMTX senere

AI:

- Ikke del av første versjon

---

# Designprinsipp

Naturblikk skal være:

- rask
- rolig
- enkel
- moderne
- naturfokusert

Livestreamen skal alltid være hovedfokuset.

---

# Første milepæl

- SSL/HTTPS
- Forside med live-plassholder
- Ett kamera
- OBS
- Stabil videostrøm

Alt annet kommer etter dette.