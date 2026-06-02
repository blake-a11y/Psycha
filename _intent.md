# _intent.md

**Phase:** 5 · **Scope:** in-scope · **Format:** Markdown with file paths

## Purpose

`Psycha` is a citation-backed knowledge repository covering **two verticals**:

1. **Psychedelic medicine and research** — compounds, mechanisms, indications, trials, regulation, institutions, funders.
2. **Longevity / human optimization** — hallmarks of aging, interventions, clinical and regulatory status, institutions, funders, commercial landscape.

For each vertical the repo also covers:
- The leading **experts** who shape the field.
- Where the field is heading over the next ~10 years.

## How this repo is used

- Files are written as Markdown so they can be loaded into a separate AI system as **advisor personas** and **field-context** modules.
- Persona files synthesize an expert's **public positions** for advisory use. They are not the real person. They do not produce quotes attributed to the real person.
- Field-context files give the AI advisor the factual ground truth it needs to reason inside the field.
- Trajectory files give the AI advisor a forward-looking frame for investment-relevant reasoning. Frame: **TSW** (Trends, Strengths, Weaknesses of incumbents), not SWOT.

## Two-vertical structure

The two verticals are **parallel**, not nested. Each has its own field-context, roster, and trajectory file. Personas live in a single `personas/` folder and are tagged by vertical in `_index.md` and the roster files.

- **Psychedelic medicine** field-context: `field-context/01–05`. Trajectory: `trajectory/10-year-outlook.md`. Roster: `roster/_roster-index.md`.
- **Longevity / human optimization** field-context: `field-context-longevity/01–06`. Trajectory: `trajectory/10-year-outlook-longevity.md`. Roster: `roster/_roster-longevity-index.md`.

Some personas are relevant to both verticals (e.g. wellness-adjacent figures). When loading an advisor, choose personas matching the question's vertical.

## Out of scope (hard limits, both verticals)

- No medical, dosing, or treatment advice.
- No guidance on obtaining, producing, or using controlled substances or unapproved compounds.
- No fabricated quotes, credentials, or trial results.
- No speculation stated as fact. Forward-looking claims labeled as estimates.
- No marketing claims (supplement, clinic, or self-experimenter) treated as validated science.

## Verification rules

- Credentials labeled `[verified]` when confirmed against primary sources (institutional pages, peer-reviewed publications, official bios).
- Labeled `[unverified]` when claimed but not confirmed.
- Credibility levels per persona: **peer-reviewed clinical**, **academic non-clinical**, **commercial / founder**, **self-experimenter / public figure**.
- Longevity-specific evidence tiers used in field-context and personas: `[validated clinical]`, `[preliminary clinical]`, `[commercial / supplement]`, `[self-experimenter / anecdotal]`.

## Source recency

- Regulatory, trial, and approval claims: sources from the last 18 months.
- General field framing: last 3–5 years acceptable.

## Loading instructions

See `_index.md` for the full file map and load order for both verticals.
