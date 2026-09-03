# Feedback Ledger

Restored durable/scoped feedback evidence. This ledger preserves high-confidence decisions needed by the current baseline; unavailable old Git history is not fabricated.

### FB-001 — Standard carousel ratio

- Evidence: explicit durable user preference
- Class: canonical-preference
- Scope: all-carousels
- Rule: standard Instagram carousel = `4:5`, target `1080×1350` unless explicitly overridden.
- Status: promoted
- Promoted to: Design Foundation / Starter

### FB-002 — Friendly-natural Persian

- Evidence: explicit durable user feedback
- Class: canonical-preference
- Scope: copy-style
- Rule: default Instagram Persian should be friendly, fluent and natural; not dry/bookish/bureaucratic.
- Status: promoted

### FB-003 — Visual sameness forbidden

- Evidence: explicit durable user feedback
- Class: negative-rule
- Scope: visual-identity
- Rule: posts must not all reuse the same colors, fonts, sizes, layout or image treatment.
- Status: promoted

### FB-004 — Category/topic-aware visual identity

- Evidence: explicit durable feedback
- Class: canonical-preference
- Scope: visual-identity
- Rule: art direction should respond to content category/topic while preserving ASDEV invariants.
- Status: promoted

### FB-005 — Footer domain

- Evidence: explicit durable user decision
- Class: canonical-preference
- Scope: final-production
- Rule: exact footer = `alirezasafaeisystems.ir`.
- Status: promoted

### FB-006 — ASDEV mark

- Evidence: explicit durable user decision
- Class: canonical-preference
- Scope: visual-identity
- Rule: ASDEV is the brand mark; visible but restrained, especially cover/closing.
- Status: promoted

### FB-007 — Meaningful visual storytelling

- Evidence: repeated specific approval
- Class: candidate-preference / promoted scoped principle
- Scope: visual-storytelling
- Rule: meaningful imagery/diagrams/visual storytelling are preferred when they improve comprehension; decoration alone is not the goal.
- Status: promoted to visual design principle

### FB-010 — Design foundation regression

- Evidence: explicit rejection of first new-chat render
- Class: system-aligned-feedback
- Scope: all-carousels / rendered-preview
- Rule: page numbering, disciplined hierarchy, consistent type sizes, alignment, spacing and understandable visuals are mandatory.
- Status: promoted
- Promoted to: REG-001 + foundation + preview gate

### FB-011 — Semantic grouping + mixed-script safety

- Evidence: explicit feedback on second new-chat render
- Class: system-aligned-feedback
- Scope: rendered-preview / visual composition
- Rule: multi-part slides need visible grouping; Persian/English composition must preserve deterministic reading order.
- Status: promoted
- Promoted to: REG-002 + semantic-region-bidi contract

### FB-013 — Phase 3 baseline accepted

- Evidence: explicit acceptance of Trial Reels new-chat output at approximately `8/10`
- Class: baseline-acceptance
- Scope: phase-3-baseline-closure
- Confidence: high
- Rule: Phase 3 is accepted/frozen; major architecture changes should now be evidence-driven.
- Status: promoted
- Notes: `8/10` is a scoped human evaluation, not Instagram performance data and does not canonicalize that post's palette/font/3D/layout surface.

### FB-014 — Talking Reel requires timed speech + real silence

- Evidence: explicit repeated feedback that continuous delivery sounded robotic; approved Gemini Live C01 used strict timed speech/silence blocks.
- Class: canonical-preference / workflow-rule
- Scope: Flow/Gemini talking-reels
- Confidence: high
- Rule: dialogue must be split into short timed speech blocks with explicit real silence; if a phrase finishes early the model must wait rather than start the next block early.
- Status: promoted
- Promoted to: `06_workflows/reels-flow-production-playbook.md` + approved prompt library

### FB-015 — Dialogue overload is a negative rule

- Evidence: explicit rejection of 8/10-second prompts with too much dialogue and repeated machine-gun outcomes.
- Class: negative-rule
- Scope: short talking-reels
- Confidence: high
- Rule: when dialogue only fits by accelerating delivery, shorten the script; do not solve density by increasing speaking speed.
- Status: promoted

### FB-016 — No-reference prompt must be self-contained

- Evidence: Gemini requested an image after prompt text referenced a provided wardrobe/reference image; user explicitly requested no reference image.
- Class: negative-rule / workflow-rule
- Scope: Flow/Gemini no-reference generation
- Confidence: high
- Rule: when no image is intended, remove all `provided image` / `reference image` language and fully describe identity, wardrobe and scene in text.
- Status: promoted

### FB-017 — Rose hair pattern is identity-critical

- Evidence: repeated explicit concern about preserving Rose identity and hair colors.
- Class: canonical-preference
- Scope: Rose visual-identity
- Confidence: high
- Rule: Rose hair lock = near-black roots + hot-magenta front/outer sections + sapphire/electric-blue underlayer; chin-length bob and black round glasses remain stable.
- Status: promoted
- Promoted to: approved prompt library

### FB-018 — Teaser Reel should preserve the curiosity gap

- Evidence: explicit user correction: the Reel should not teach the method; it should bring the viewer to Telegram for the tutorial.
- Class: canonical-preference / funnel-rule
- Scope: Telegram-funnel Reels
- Confidence: high
- Rule: teaser Reel = problem + promise + destination; technical method belongs in Telegram/PDF/caption when depth is needed.
- Status: promoted

### FB-019 — Cover headline must be understandable to general audience

- Evidence: explicit rejection of visually strong cover whose headline was not meaningful to general viewers; subsequent outcome-first cover direction approved.
- Class: canonical-preference
- Scope: Reel covers
- Confidence: high
- Rule: cover must communicate the outcome without requiring prior knowledge of Flow/model names; technical context may be secondary, outcome is the dominant headline.
- Status: promoted

### FB-020 — Telegram CTA requires edit-safe pointing space

- Evidence: explicit request that presenter point down while saying Telegram so channel ID can be added in edit.
- Class: workflow-rule
- Scope: Telegram-funnel talking-reels
- Confidence: high
- Rule: on `کانال تلگرام`, one index finger points clearly to lower-center; lower-center stays empty; final pose holds ~0.5–0.8s; generated username/logo/arrow are forbidden.
- Status: promoted

### FB-021 — Limited-credit mode uses one-shot prompt design

- Evidence: explicit user statement that additional credits/cost for trial-and-error were not available.
- Class: conditional-workflow-rule
- Scope: Flow/Gemini tasks when user states credit/budget constraint
- Confidence: high
- Rule: provide one best production prompt, self-audit timing/reference/pronunciation before render, and do not propose speculative A/B generations unless requested.
- Status: promoted-scoped

## Ledger Rules

- broad rule without durable/repeated evidence is forbidden;
- every durable entry needs source/scope;
- preferences can be superseded rather than deleted;
- do not invent performance metrics.

## Next ID

`FB-022`
