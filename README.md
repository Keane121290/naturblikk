# 🌿 Naturblikk

**Et vindu mot norsk natur.**

Naturblikk er et norsk natur- og livestreamprosjekt som starter med en fuglemater på Helgeland. Målet er å lage en rolig, tilgjengelig og moderne nettside der besøkende kan følge fuglelivet direkte – og etter hvert utforske arter, historikk, værdata og statistikk.

Prosjektet starter enkelt med WordPress, to utendørskameraer og livestream direkte på forsiden. Over tid kan løsningen vokse til en mer avansert plattform med egen streamingmotor, AI-basert artsgjenkjenning og historikk.

---

## Status

🚧 **Under utvikling**

WordPress er installert på:

```text
https://naturblikk.no
```

Neste hovedoppgave er SSL/HTTPS, globalt designoppsett i Kadence og bygging av forsiden.

---

## Visjon

Naturblikk skal gi folk et lite pusterom i hverdagen – et sted hvor man kan åpne nettsiden og se ekte natur i sanntid.

Ikke støy.  
Ikke klikkjag.  
Bare norsk natur, fugleliv og små øyeblikk.

---

## Første versjon

- Enkel, moderne WordPress-side
- Livestream direkte på forsiden
- Informasjon om prosjektet
- Mobilvennlig design
- Diskré og bærekraftig annonseplassering senere

---

## Senere versjoner

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
│   ├── Forside med livestream
│   ├── Om prosjektet
│   ├── Arter
│   ├── Galleri
│   ├── Kontakt
│   └── Personvern
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
├── frontend/       # Designreferanse og fremtidig frontend/webapp
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
- [x] WordPress installert
- [x] Kadence Theme installert
- [x] Kadence Blocks installert
- [ ] SSL/HTTPS aktivert
- [ ] Første forside publisert

### v0.2 – Første live-forside

- [ ] Lage midlertidig live-placeholder på forsiden
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
- [ ] Om-side
- [ ] Kontaktinformasjon
- [ ] Personvern
- [ ] Enkel driftsrutine

---

## Teknologi

Foreløpig plan:

- **WordPress** – første nettside og innhold
- **Kadence** – lett og moderne WordPress-tema
- **OBS** – miksing av kamera, lyd og overlay
- **MediaMTX** – fremtidig egen streamingserver
- **Python** – AI og analyse senere
- **SQLite/PostgreSQL** – historikk og statistikk senere

---

## Designretning

Naturblikk skal føles:

- rolig
- nordisk
- naturlig
- moderne
- lite påtrengende

Mer detaljer ligger i `docs/branding.md` og `docs/style-guide.md`.

---

## Lisens

Prosjektet er foreløpig lisensiert under MIT-lisensen. Se `LICENSE`.

---

## Prosjektstatus

Naturblikk er et aktivt hobbyprosjekt under oppbygging.

Første milepæl er å få opp en enkel forside med livestream. Etter det bygges prosjektet videre steg for steg.