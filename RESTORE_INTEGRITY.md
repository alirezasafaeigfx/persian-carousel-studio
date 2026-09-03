# Restore Integrity Manifest

Date: 2026-09-03
Repository: `alirezasafaeigfx/persian-carousel-studio`

## Purpose

This document records the integrity checks performed after restoring Persian Carousel Studio from the unavailable previous GitHub account.

It complements `MIGRATION.md`:

- `MIGRATION.md` explains **why** restoration was required and what historical data could not be recovered.
- this file records **what operational baseline is present and verified now**.

## Authority

From this migration onward, the authoritative Source of Truth is:

`https://github.com/alirezasafaeigfx/persian-carousel-studio`

The previous owner/repository must not be used by runtime prompts, starter templates or new project documentation.

## Verified Runtime Baseline

The restored repository contains the six baseline full-carousel references:

1. `01_brand/brand-voice.md`
2. `02_persian-language/persian-style-guide.md`
3. `03_content-system/carousel-narrative-system.md`
4. `04_design-system/visual-design-system.md`
5. `05_quality-control/anti-ai-qa.md`
6. `07_templates/carousel-output-schema.md`

`07_templates/chat-starter-template.md` remains the runtime router/orchestrator and points to the new repository owner.

## Verified Design / Render Contracts

Present and routable:

- `04_design-system/carousel-foundation-tokens.md`
- `04_design-system/semantic-region-bidi-contract.md`
- `05_quality-control/rendered-preview-gate.md`
- `05_quality-control/final-render-verification.md`
- `06_workflows/preview-to-final-workflow.md`
- `11_prompt-libraries/image-prompt-library.md`
- `11_prompt-libraries/render-foundation-prompt-contract.md`

Regression evidence restored:

- `05_quality-control/regressions/REG-001-new-chat-render-design-foundation.md`
- `05_quality-control/regressions/REG-002-semantic-framing-bidi.md`

## Verified Identity / Learning Contracts

Present and routable:

- `08_examples/gold-standard-registry.md`
- `08_examples/gold-standards/GS-001-pilot-001-preview-direction.md`
- `09_brand-identity/visual-identity-grammar.md`
- `09_brand-identity/category-art-direction-system.md`
- `09_brand-identity/visual-variation-router.md`
- `09_brand-identity/recent-style-exclusion.md`
- `10_feedback-learning/feedback-learning-protocol.md`
- `10_feedback-learning/feedback-ledger.md`

## Verified Marketing / Copy Contracts

Present and routable:

- `12_marketing/content-category-system.md`
- `12_marketing/marketing-objective-system.md`
- `12_marketing/content-funnel.md`
- `12_marketing/cta-strategy.md`
- `13_copywriting/instagram-copywriting-system.md`
- `13_copywriting/hook-headline-system.md`
- `13_copywriting/persuasion-and-claim-discipline.md`
- `13_copywriting/cta-copy-system.md`

## Verified Observation Memory

Present:

- `14_observations/README.md`
- `14_observations/post-observation-template.md`
- `14_observations/recent-post-index.md`
- `14_observations/posts/README.md`
- `14_observations/synthesis/README.md`

Memory policy remains:

- **Hot:** baseline + task-routed canonical references
- **Warm:** recent-post index only when recent-style evidence is needed
- **Cold:** individual observations, synthesis, regression history, acceptance/governance history

Whole-repository loading remains prohibited for ordinary carousel generation.

## Verified Governance State

Current operational status:

- Phase 1 — `COMPLETE`
- Phase 2 — `COMPLETE`
- Phase 3 — `ACCEPTED / FROZEN`
- Production Observation Memory — `ACTIVE`
- Phase 4 — `DEFERRED / EVIDENCE-GATED`

Governance and acceptance documents are present under:

- `docs/acceptance/`
- `docs/governance/`

They are evidence/cold-path documents, not default runtime context.

## Migration Checks Completed

- `main` resolves to the restored operational tree.
- runtime Starter references the new repository owner.
- Prompt Library, Marketing, Copywriting, Observation and Synthesis directories were independently enumerated after restore.
- code search for `alirezasafaei-dev` in the new repository returned no active matches.
- Observation recent index starts without fabricated historical entries.
- no `AGENTS.md` was introduced.
- no Phase 4 implementation was added during migration.

## Known Non-Recoverable History

The following are **not** claimed to have been restored:

- exact commit graph from the previous account;
- old PR/review metadata as GitHub objects;
- historical branches and tags;
- byte-for-byte copies of every old Superpowers spec/plan.

These gaps do not change the authority of the restored current operational baseline.

## Restore Baseline Commit

Initial restored operational baseline commit:

`1e62e8d52aa000745ef0634f09a54532c06654f2`

Later documentation-only hardening commits may follow this SHA without reopening Phase 3 scope.

## Operating Rule After Migration

> Build posts from the new Source of Truth, record real evidence, and change architecture only when a demonstrated defect or repeated evidence justifies it.
