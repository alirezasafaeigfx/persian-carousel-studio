# REG-002 — Semantic Framing + Bidi

Status: `GREEN`

## Failure observed

The next fresh-chat test materially improved hierarchy and numbering but exposed:

1. multi-part slides visually floating without enough grouping;
2. Persian + Latin/code text breaking in image rendering.

Examples included mixed runs similar to `۳) OPTIONS:` and unsafe hybrid morphology.

## Root cause

Grid discipline alone did not define semantic regions, and atomic-token guidance was insufficient for image-generation bidi behavior.

## Fix

- Semantic Region Grammar;
- framing strength `F0–F3`;
- visible grouping requirement for multi-region slides;
- explicit Bidi Plan;
- critical Persian/LTR text split into separate visual elements;
- exact-text bidi isolation;
- Persian copy-stage avoidance of unsafe hybrid words;
- artifact-level framing and bidi QA.

## Regression expectation

Unframed multi-region slides and broken mixed-direction token order are MAJOR defects and cannot pass preview QA.
