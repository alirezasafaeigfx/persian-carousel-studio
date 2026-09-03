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

## Ledger Rules

- broad rule without durable/repeated evidence is forbidden;
- every durable entry needs source/scope;
- preferences can be superseded rather than deleted;
- do not invent performance metrics.

## Next ID

`FB-014`
