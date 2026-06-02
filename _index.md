# _index.md — Master index and load instructions

**Phase:** 5 · **Scope:** in-scope · **Format:** Markdown with file paths

This repo covers **two verticals**: psychedelic medicine and longevity / human optimization. Each has its own field-context, roster, and trajectory. Personas live in a single `personas/` folder, tagged by vertical below.

## File map

### Repo meta
- [`README.md`](README.md)
- [`_intent.md`](_intent.md) — why this repo exists; rules
- [`_index.md`](_index.md) — this file
- [`_templates/persona-template.md`](_templates/persona-template.md)
- [`_templates/field-context-template.md`](_templates/field-context-template.md)
- [`_templates/trajectory-template.md`](_templates/trajectory-template.md)

### Vertical A — Psychedelic medicine

**Field context (Phase 1):**
- [`field-context/01-what-is-psychedelic-medicine.md`](field-context/01-what-is-psychedelic-medicine.md)
- [`field-context/02-compounds-and-mechanisms.md`](field-context/02-compounds-and-mechanisms.md)
- [`field-context/03-therapeutic-indications.md`](field-context/03-therapeutic-indications.md)
- [`field-context/04-trial-and-regulatory-landscape.md`](field-context/04-trial-and-regulatory-landscape.md)
- [`field-context/05-institutions-and-funders.md`](field-context/05-institutions-and-funders.md)

**Roster (Phase 2):**
- [`roster/_roster-index.md`](roster/_roster-index.md)

**Personas (Phase 3):**
- [`personas/carhart-harris-robin.md`](personas/carhart-harris-robin.md)
- [`personas/rabin-david.md`](personas/rabin-david.md)
- [`personas/doblin-rick.md`](personas/doblin-rick.md)
- [`personas/nutt-david.md`](personas/nutt-david.md)
- [`personas/johnson-matthew.md`](personas/johnson-matthew.md)
- [`personas/raison-charles.md`](personas/raison-charles.md)
- [`personas/yehuda-rachel.md`](personas/yehuda-rachel.md)
- [`personas/griffiths-roland.md`](personas/griffiths-roland.md) — posthumous
- [`personas/ross-stephen.md`](personas/ross-stephen.md)
- [`personas/nath-kabir.md`](personas/nath-kabir.md)
- [`personas/feilding-amanda.md`](personas/feilding-amanda.md)

**Trajectory (Phase 4):**
- [`trajectory/10-year-outlook.md`](trajectory/10-year-outlook.md)

### Vertical B — Longevity / human optimization

**Field context (Phase L1):**
- [`field-context-longevity/01-what-is-longevity-human-optimization.md`](field-context-longevity/01-what-is-longevity-human-optimization.md)
- [`field-context-longevity/02-hallmarks-and-mechanisms-of-aging.md`](field-context-longevity/02-hallmarks-and-mechanisms-of-aging.md)
- [`field-context-longevity/03-intervention-landscape-and-evidence-tiers.md`](field-context-longevity/03-intervention-landscape-and-evidence-tiers.md)
- [`field-context-longevity/04-clinical-and-regulatory-status.md`](field-context-longevity/04-clinical-and-regulatory-status.md)
- [`field-context-longevity/05-institutions-and-funders.md`](field-context-longevity/05-institutions-and-funders.md)
- [`field-context-longevity/06-commercial-landscape.md`](field-context-longevity/06-commercial-landscape.md)

**Roster (Phase L2):**
- [`roster/_roster-longevity-index.md`](roster/_roster-longevity-index.md)

**Personas (Phase L3):**
- [`personas/sinclair-david.md`](personas/sinclair-david.md)
- [`personas/johnson-bryan.md`](personas/johnson-bryan.md)
- [`personas/barzilai-nir.md`](personas/barzilai-nir.md)
- [`personas/horvath-steve.md`](personas/horvath-steve.md)
- [`personas/lopez-otin-carlos.md`](personas/lopez-otin-carlos.md)
- [`personas/attia-peter.md`](personas/attia-peter.md)
- [`personas/kaeberlein-matt.md`](personas/kaeberlein-matt.md)
- [`personas/blasco-maria.md`](personas/blasco-maria.md)
- [`personas/verdin-eric.md`](personas/verdin-eric.md)
- [`personas/levine-morgan.md`](personas/levine-morgan.md)
- [`personas/yamanaka-shinya.md`](personas/yamanaka-shinya.md)
- [`personas/gladyshev-vadim.md`](personas/gladyshev-vadim.md)
- [`personas/kirkland-james.md`](personas/kirkland-james.md)
- [`personas/kennedy-brian.md`](personas/kennedy-brian.md)
- [`personas/partridge-linda.md`](personas/partridge-linda.md)
- [`personas/belsky-daniel.md`](personas/belsky-daniel.md)
- [`personas/huberman-andrew.md`](personas/huberman-andrew.md)
- [`personas/patrick-rhonda.md`](personas/patrick-rhonda.md)

**Trajectory (Phase L4):**
- [`trajectory/10-year-outlook-longevity.md`](trajectory/10-year-outlook-longevity.md)

## Recommended load order into an AI advisor

Same pattern for either vertical. Replace paths with the vertical's files.

1. **Frame first.** Load `_intent.md` — defines scope, hard limits, verification rules. Everything below inherits from it.
2. **Ground truth.** Load all field-context files for the active vertical. The advisor must speak the field accurately before it speaks any expert's voice.
   - Psychedelic: `field-context/01–05`
   - Longevity: `field-context-longevity/01–06`
3. **Roster context.** Load the matching roster index for a relative-influence map.
   - Psychedelic: `roster/_roster-index.md`
   - Longevity: `roster/_roster-longevity-index.md`
4. **Personas (one or many).** Load `personas/*.md` selectively. Choose personas matching the question's vertical.
   - Panel-style advisor: load 3–5 personas representing different stances. Examples:
     - Psychedelic panel: Carhart-Harris + Raison + Nath + Doblin + Yehuda.
     - Longevity panel: Barzilai + Kaeberlein + Sinclair + Attia + Kirkland.
   - Single-perspective advisor: load 1 persona only.
5. **Forward view last.** Load the matching trajectory file only when forward-looking, investment-flavored questions are in play. Load with explicit instruction: "Forward-looking claims are estimates, not facts."
   - Psychedelic: `trajectory/10-year-outlook.md`
   - Longevity: `trajectory/10-year-outlook-longevity.md`

**Do not mix verticals in one advisor session unless the question explicitly spans both.** Mixing dilutes the field-context and produces hedged, generic answers.

## How to instantiate a persona

Recommended system-prompt fragment when loading a persona file:

```
You are an advisor synthesizing the public positions of [NAME] as documented in [persona-file].
You are NOT [NAME]. You do not generate fabricated quotes or claim to speak as them.
Use their reasoning style, evidence base, and known positions to advise.
Disclose biases, financial interests, and credibility limits from the persona file when relevant to the question.
Defer to field-context files for factual claims. Defer to trajectory file for forward-looking estimates.
Refuse medical, dosing, or treatment advice.
```

## Update cadence

- Trial / regulatory facts (field-context 04, longevity 04, both trajectories): refresh every 90 days.
- Persona files: refresh on any major event (publication, board change, public position change, financial-interest change).
- Roster rankings: review every 6 months.

## Cross-vertical notes

- The longevity trajectory (`trajectory/10-year-outlook-longevity.md`) includes an explicit comparison table to psychedelic commercialization. Useful when the same investor or operator is evaluating both verticals.
- Personas with public positions in both verticals are tagged in each vertical's roster. Currently none in the seed set; revisit if added.

## Open items for the repo owner

1. Decide whether to expand either vertical's persona set further.
2. Decide retention policy if a vertical is later narrowed or removed.
3. Decide whether to add a third vertical (e.g. metabolic health, mental performance) under the same parallel structure.
