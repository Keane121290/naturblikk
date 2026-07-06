# 🌿 Naturblikk

**Et vindu mot norsk natur.**

Naturblikk er et norsk natur- og livestreamprosjekt som starter med en fuglemater på Helgeland. Målet er å lage en rolig, tilgjengelig og moderne nettside der besøkende kan følge fuglelivet direkte – og etter hvert utforske arter, historikk, værdata og statistikk.

Prosjektet starter enkelt med WordPress, to utendørskameraer og en live-side. Over tid skal løsningen kunne vokse til en mer avansert plattform med egen streamingmotor, AI-basert artsgjenkjenning og historikk.

---

## Status

🚧 **Under utvikling**

Første mål er å få opp en enkel nettside på:

```text
https://naturblikk.no
```

Deretter kobles første livestream til når kameraene er klare.

---

## Visjon

Naturblikk skal gi folk et lite pusterom i hverdagen – et sted hvor man kan åpne nettsiden og se ekte natur i sanntid.

Ikke støy.  
Ikke klikkjag.  
Bare norsk natur, fugleliv og små øyeblikk.

---

## Planlagte funksjoner

### Første versjon

- Enkel, moderne nettside
- Live-side klar for videostrøm
- Informasjon om prosjektet
- Mobilvennlig design
- Grunnleggende WordPress-oppsett

### Senere versjoner

- 📺 Livestream fra fuglemater
- 🎥 Flere kameravinkler
- 🐦 AI-basert artsgjenkjenning
- 📊 Statistikk over observasjoner
- 🌦️ Værdata fra området
- 📅 Historikk og dagbok
- 📸 Bilder og høydepunkter
- 🔇 Kontrollert lydmodus med mulighet for tale-demping

---

## Foreslått arkitektur

```text
Naturblikk.no
│
├── WordPress
│   ├── Forside
│   ├── Live
│   ├── Om
│   └── Nyheter
│
├── Stream
│   ├── Kameraer
│   ├── OBS
│   └── MediaMTX
│
├── AI
│   ├── Artsgjenkjenning
│   ├── Lydanalyse
│   └── Hendelser
│
└── Backend
    ├── API
    ├── Database
    ├── Statistikk
    └── Værdata
```

WordPress brukes i starten som nettside og innholdsplattform. Streaming, AI og statistikk kan bygges som egne moduler etter hvert.

---

## Repository-struktur

```text
naturblikk/
│
├── ai/             # AI, artsgjenkjenning og lydanalyse
├── assets/         # Logo, bilder, ikoner og grafikk
├── backend/        # API, database og serverlogikk
├── docs/           # Dokumentasjon, roadmap og arkitektur
├── frontend/       # Fremtidig egen frontend/webapp
├── obs/            # OBS-profiler, scener og notater
├── scripts/        # Hjelpeskript og automatisering
├── stream/         # MediaMTX, RTSP, WebRTC og streamingoppsett
├── wordpress/      # WordPress-notater, tema og tilpasninger
│
├── .gitignore
├── LICENSE
└── README.md
```

---

## Roadmap

### v0.1 – Grunnmur

- [x] Prosjektnavn valgt
- [x] Domene registrert
- [x] GitHub-repository opprettet
- [x] Grunnstruktur opprettet
- [ ] WordPress installert
- [ ] Første forside publisert

### v0.2 – Første live-side

- [ ] Opprette `/live`
- [ ] Lage midlertidig live-placeholder
- [ ] Klargjøre layout for videospiller
- [ ] Teste mobilvisning

### v0.3 – Kamera og stream

- [ ] Koble til første Tapo C310
- [ ] Hente RTSP-strøm
- [ ] Teste OBS
- [ ] Teste MediaMTX
- [ ] Vise første livebilde på nettsiden

### v0.4 – Utvidelser

- [ ] Kamera 2
- [ ] Grunnleggende værdata
- [ ] Enkle observasjonsnotater
- [ ] Første versjon av statistikk

### v1.0 – Offisiell lansering

- [ ] Stabil livestream
- [ ] Ferdig forside
- [ ] Live-side
- [ ] Om-side
- [ ] Kontaktinformasjon
- [ ] Enkel driftsrutine

---

## Teknologi

Foreløpig plan:

- **WordPress** – første nettside og innhold
- **Kadence** – lett og moderne WordPress-tema
- **OBS** – miksing av kamera, lyd og overlay
- **MediaMTX** – fremtidig egen streamingserver
- **Python** – AI og analyse
- **SQLite/PostgreSQL** – historikk og statistikk senere

---

## Designretning

Naturblikk skal føles:

- rolig
- nordisk
- naturlig
- moderne
- lite påtrengende

Foreslått uttrykk:

```text
Primærfarge:   Dyp grønn/blå
Sekundær:      Mosegrønn
Bakgrunn:      Varm hvit
Typografi:     Enkel og moderne
```

Mer detaljer ligger etter hvert i `docs/branding.md`.

---

## Lisens

Prosjektet er foreløpig lisensiert under MIT-lisensen. Se `LICENSE`.

---

## Prosjektstatus

Naturblikk er et aktivt hobbyprosjekt under oppbygging.

Første milepæl er å få opp en enkel nettside og en stabil livestream. Etter det bygges prosjektet videre steg for steg.
