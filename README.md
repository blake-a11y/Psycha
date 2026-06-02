# Psycha

Citation-backed knowledge repository covering two verticals: **psychedelic medicine** and **longevity / human optimization**. Files are Markdown, loadable as advisor personas and field-context modules into an AI advisor system.

See [`_intent.md`](_intent.md) for scope, rules, and verification standards.
See [`_index.md`](_index.md) for the master file map and load order for both verticals.

## Verticals

| Vertical | Field context | Roster | Trajectory | Personas |
|---|---|---|---|---|
| Psychedelic medicine | `field-context/01–05` | `roster/_roster-index.md` | `trajectory/10-year-outlook.md` | 11 |
| Longevity / human optimization | `field-context-longevity/01–06` | `roster/_roster-longevity-index.md` | `trajectory/10-year-outlook-longevity.md` | 18 |

## Folder tree

```
Psycha/
├── README.md
├── _intent.md
├── _index.md                              # master index + load instructions
├── _templates/
│   ├── persona-template.md
│   ├── field-context-template.md
│   └── trajectory-template.md
├── field-context/                         # Vertical A: psychedelic medicine
│   ├── 01-what-is-psychedelic-medicine.md
│   ├── 02-compounds-and-mechanisms.md
│   ├── 03-therapeutic-indications.md
│   ├── 04-trial-and-regulatory-landscape.md
│   └── 05-institutions-and-funders.md
├── field-context-longevity/               # Vertical B: longevity
│   ├── 01-what-is-longevity-human-optimization.md
│   ├── 02-hallmarks-and-mechanisms-of-aging.md
│   ├── 03-intervention-landscape-and-evidence-tiers.md
│   ├── 04-clinical-and-regulatory-status.md
│   ├── 05-institutions-and-funders.md
│   └── 06-commercial-landscape.md
├── roster/
│   ├── _roster-index.md                   # psychedelic
│   └── _roster-longevity-index.md         # longevity
├── personas/                              # both verticals, tagged in _index.md
│   ├── (psychedelic — 11 files)
│   └── (longevity — 18 files)
└── trajectory/
    ├── 10-year-outlook.md                 # psychedelic
    └── 10-year-outlook-longevity.md       # longevity
```

## Status

| Phase | Vertical A (psychedelic) | Vertical B (longevity) |
|---|---|---|
| Architecture, templates, intent | complete | complete |
| Field-context files | complete (5) | complete (6) |
| Roster index | complete | complete |
| Per-expert personas | complete (11) | complete (18) |
| Trajectory | complete | complete |
| Master index + load instructions | complete | complete |

## Usage rules (summary)

- No medical, dosing, or treatment advice.
- No fabricated quotes or credentials.
- Forward-looking claims are estimates, not facts.
- Do not mix verticals in one advisor session unless the question explicitly spans both.

Full rules in [`_intent.md`](_intent.md).
