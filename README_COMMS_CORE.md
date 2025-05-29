# COMMS Core – Agentmodell V1

Dette repoet inneholder kjernestrukturen for COMMS Agentmodell V1 – et dynamisk Multi-Agent-system for ledelsesstøtte, analyse og organisatorisk struktur.

## 📁 Mappestruktur

```
/
├── actions/                  ← JSON-filer som definerer agentenes handlinger
├── definitions/              ← Skjemaer, metadata og strukturstandarder
├── docs/                     ← Valgfri dokumentasjon eller GitHub Pages
├── .github/workflows/        ← GitHub Actions for validering og automatisering
├── .devcontainer/            ← Konfig for Codespaces/prebuilds
└── README.md                 ← Denne filen
```

## 🧰 Bruksområder

- Utvikle og teste GPT-handlinger
- Standardisere input/output for AI-agenter
- Dokumentere roller, prosesser og datastruktur
- Automatisere validering av JSON via GitHub Actions

## 📦 Innhold

### `actions/`
- Inneholder en `.json` per GPT-handling
- Filnavn følger konvensjon: `STV-COMMS-05-AC-[AGT]-[LNR]-[REV].json`

### `definitions/`
- `schema-action-v1.json`: Skjemadefinisjon for handlingsfiler
- `agent-roles.yml`: Beskrivelse av agentroller
- `input-output-types.md`: Standardverdier
- `example-valid-action.json`: Referanseeksempel

### `.github/workflows/`
- Inneholder GitHub Actions som validerer at `actions/*.json` følger skjema

## 🛠️ Kom i gang

1. Klon repo:
```bash
git clone https://github.com/[brukernavn]/comms-core.git
cd comms-core
```

2. Legg til en ny action:
   - Lag ny fil i `actions/`
   - Valider mot `definitions/schema-action-v1.json`

3. Opprett et GitHub Project for fremdriftsstyring

## 🔒 Privacy og GPT-integrasjon

Bruk `privacy.md` i rotkatalog som Privacy URL ved GPT-handlinger.

## 📬 Kontakt

Henrik Strand  
Avdelingsleder og systemeier  
henrik-l.strand@gk.no
