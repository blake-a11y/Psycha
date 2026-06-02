# _index.md — Master index and load instructions

**Phase:** 5 · **Scope:** in-scope · **Format:** Markdown with file paths

## File map

### Repo meta
- [`README.md`](README.md)
- [`_intent.md`](_intent.md) — why this repo exists; rules
- [`_index.md`](_index.md) — this file
- [`_templates/persona-template.md`](_templates/persona-template.md)
- [`_templates/field-context-template.md`](_templates/field-context-template.md)
- [`_templates/trajectory-template.md`](_templates/trajectory-template.md)

### Phase 1 — Field context
- [`field-context/01-what-is-psychedelic-medicine.md`](field-context/01-what-is-psychedelic-medicine.md)
- [`field-context/02-compounds-and-mechanisms.md`](field-context/02-compounds-and-mechanisms.md)
- [`field-context/03-therapeutic-indications.md`](field-context/03-therapeutic-indications.md)
- [`field-context/04-trial-and-regulatory-landscape.md`](field-context/04-trial-and-regulatory-landscape.md)
- [`field-context/05-institutions-and-funders.md`](field-context/05-institutions-and-funders.md)

### Phase 2 — Roster
- [`roster/_roster-index.md`](roster/_roster-index.md)

### Phase 3 — Personas
Seed:
- [`personas/carhart-harris-robin.md`](personas/carhart-harris-robin.md)
- [`personas/rabin-david.md`](personas/rabin-david.md)
- [`personas/sinclair-david.md`](personas/sinclair-david.md) `[adjacent — longevity]`
- [`personas/johnson-bryan.md`](personas/johnson-bryan.md) `[adjacent — longevity]`

Discovered (psychedelic medicine):
- [`personas/doblin-rick.md`](personas/doblin-rick.md)
- [`personas/nutt-david.md`](personas/nutt-david.md)
- [`personas/johnson-matthew.md`](personas/johnson-matthew.md)
- [`personas/raison-charles.md`](personas/raison-charles.md)
- [`personas/yehuda-rachel.md`](personas/yehuda-rachel.md)
- [`personas/griffiths-roland.md`](personas/griffiths-roland.md) — posthumous
- [`personas/ross-stephen.md`](personas/ross-stephen.md)
- [`personas/nath-kabir.md`](personas/nath-kabir.md)
- [`personas/feilding-amanda.md`](personas/feilding-amanda.md)

### Phase 4 — Trajectory
- [`trajectory/10-year-outlook.md`](trajectory/10-year-outlook.md)

## Recommended load order into an AI advisor

1. **Frame first.** Load `_intent.md` — defines scope, hard limits, verification rules. Everything below inherits from it.
2. **Ground truth.** Load all five `field-context/` files. The advisor must speak the field accurately before it speaks any expert's voice.
3. **Roster context.** Load `roster/_roster-index.md` so the advisor has a relative-influence map.
4. **Personas (one or many).** Load `personas/*.md` selectively, depending on use:
   - For a panel-style advisor: load 3–5 personas representing different stances (e.g. Carhart-Harris + Raison + Nath + Doblin + Yehuda).
   - For single-perspective advisor: load 1 persona only.
   - Always pair longevity-adjacent personas (Sinclair, Johnson) with `_intent.md`'s scope-deviation note so the advisor maintains the distinction.
5. **Forward view last.** Load `trajectory/10-year-outlook.md` only when forward-looking, investment-flavored questions are in play. Load with explicit instruction: "Forward-looking claims are estimates, not facts."

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

- Trial / regulatory facts (field-context 04, trajectory): refresh every 90 days.
- Persona files: refresh on any major event (publication, board change, public position change).
- Roster ranking: review every 6 months.

## Open items for the repo owner

1. Confirm the 4th seed identity (best-fit selected: Robin Carhart-Harris).
2. Decide whether to expand the adjacent (longevity) section beyond Sinclair / Johnson — e.g. Peter Attia, Andrew Huberman, Rhonda Patrick.
3. Decide retention policy for `[adjacent]` personas if scope is later re-narrowed.
