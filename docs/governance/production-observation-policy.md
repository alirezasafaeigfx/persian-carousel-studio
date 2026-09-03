# Production Observation / Change Governance Policy

Status: active after Phase 3 closure and repository restoration.

## Purpose

The next goal is not to add rules by default; it is to observe the system in real use and change architecture only when evidence justifies it.

> **Use → observe → collect evidence → fix demonstrated defects.**

## Freeze Rule

The default carousel-generation hot path is frozen.

A baseline behavior change requires at least one of:

1. reproducible regression from real production/new-chat test;
2. explicit durable user feedback with clear scope;
3. repeated evidence across multiple posts;
4. correctness, claim-integrity, factual, brand-signature or publication-blocking defect.

## Not enough by itself

- theoretically useful idea;
- fashionable design technique;
- preference inferred from one successful post;
- feature that might be useful later;
- documentation added only to appear comprehensive.

## Observation target

Before reopening major architecture work, target at least **10 real carousel production tests** across different content situations.

Prefer coverage across CAT-01 through CAT-06.

A serious correctness defect may be fixed immediately before ten tests.

## Evidence unit

Preferred real-production evidence:

`14_observations/posts/OBS-NNN-<slug>.md`

Observation is evidence, not a canonical rule.

## Memory architecture

Warm during ordinary work only when needed:

- `14_observations/recent-post-index.md`

Cold by default:

- individual observations;
- synthesis history;
- regressions;
- acceptance/governance history;
- development specs/plans.

## Hot-path budget

Repository size may grow. Default context should not grow with it.

A normal carousel task must **never require whole-repository loading**.

## Checkpoints

- 10 observations → SYN-010
- 20 observations → SYN-020

Synthesis does not auto-promote rules.

## Phase 4

`DEFERRED / EVIDENCE-GATED`

Reopen only when real repeated use demonstrates needs such as delivery packs, performance learning from real data, content operations, planning/calendar, recurring archetypes, or deliberate publishing scope expansion.

If implemented, Phase 4 must be task-routed/opt-in and never added to the default full-carousel baseline merely because files exist.

## Regression policy

1. reproduce failure;
2. identify earliest layer that should have prevented it;
3. create narrow regression record;
4. fix root contract;
5. verify no unnecessary template or baseline dependency was created.

## Repository authority

Current Source of Truth:

`https://github.com/alirezasafaeigfx/persian-carousel-studio`

Migration details: `MIGRATION.md`.
