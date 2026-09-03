# Repository Migration

Date: 2026-09-03

## Why this repository exists

The previous Source-of-Truth repository lived at:

`alirezasafaei-dev/persian-carousel-studio`

After the previous GitHub account became unavailable, GitHub API access to that repository returned `404`. The old repository's Git objects and commit history therefore could not be transferred directly.

## What was restored

This repository restores the **current accepted operational baseline** from preserved project evidence in connected ChatGPT conversations, Library artifacts, Notion documentation, accepted regression decisions, and the latest canonical contracts that had been reviewed before the old account became unavailable.

Restored state:

- Phase 1: COMPLETE
- Phase 2: COMPLETE
- Phase 3: ACCEPTED / FROZEN
- Production Observation Memory: ACTIVE
- Phase 4: DEFERRED / EVIDENCE-GATED

## What was not recoverable

- exact historical Git commit graph from the old repository;
- old PR metadata and branch history as repository objects;
- byte-for-byte copies of every historical Superpowers spec/plan.

The functional Source of Truth is restored here. Historical facts that cannot be verified are not fabricated.

## New authority

From this migration onward, the authoritative repository is:

`https://github.com/alirezasafaeigfx/persian-carousel-studio`

All new observations, regressions, rules and production changes must target this repository.
