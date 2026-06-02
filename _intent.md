# _intent.md

**Phase:** 0 · **Scope:** in-scope · **Format:** Markdown with file paths

## Purpose

`Psycha` is a citation-backed knowledge repository covering:

1. The field of **psychedelic medicine and research** — compounds, mechanisms, indications, trials, regulation, institutions, funders.
2. The leading **experts** who shape that field, plus adjacent **longevity / human-optimization** experts requested by the repo owner (scope deviation noted below).
3. Where the field is heading over the next ~10 years.

## How this repo is used

- Files are written as Markdown so they can be loaded into a separate AI system as **advisor personas** and **field-context** modules.
- Persona files synthesize an expert's **public positions** for advisory use. They are not the real person. They do not produce quotes attributed to the real person.
- Field-context files give the AI advisor the factual ground truth it needs to reason inside the field.
- The trajectory file gives the AI advisor a forward-looking frame for investment-relevant reasoning.

## Out of scope (hard limits)

- No medical, dosing, or treatment advice.
- No guidance on obtaining, producing, or using controlled substances.
- No fabricated quotes, credentials, or trial results.
- No speculation stated as fact. Forward-looking claims labeled as estimates.

## Scope deviation (acknowledged)

The seed roster includes **Dr. David Sinclair** (Harvard, longevity genetics) and **Bryan Johnson** (Project Blueprint, longevity self-experimentation). Neither is a psychedelic researcher. Per repo-owner direction, scope is broadened to **psychedelic medicine + longevity / human optimization**. Field-context files remain psychedelic-medicine-first; longevity context appears only in the personas of those two experts.

## Verification rules

- Credentials labeled `[verified]` when confirmed against primary sources (institutional pages, peer-reviewed publications, official bios).
- Labeled `[unverified]` when claimed but not confirmed.
- Credibility levels per persona: **peer-reviewed clinical**, **academic non-clinical**, **commercial / founder**, **self-experimenter / public figure**.

## Source recency

- Regulatory, trial, and approval claims: sources from the last 18 months.
- General field framing: last 3–5 years acceptable.

## Loading instructions

See `_index.md` (Phase 5) for the load order and how to mount persona files into an AI advisor.
