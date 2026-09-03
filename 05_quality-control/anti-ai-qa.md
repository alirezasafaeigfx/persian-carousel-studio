# Anti-AI QA

Run adversarial QA before calling a carousel ready.

## Result states

`PASS | REVISE | INCOMPLETE`

Severity:

- `BLOCKER` — cannot ship
- `MAJOR` — must fix before presenting as production candidate
- `MINOR` — polish issue

## Content / claim checks

- fake fact/source/metric → BLOCKER
- unsupported percentage/multiplier/ranking/magnitude → BLOCKER
- universal claims like «همه/هیچ‌کس» without basis → revise/block depending on materiality
- clickbait promise not paid off → MAJOR
- exact approved copy silently rewritten → BLOCKER

## Persian checks

- dry/translated/bureaucratic Persian
- broken grammar or spelling
- mixed RTL/LTR order defects
- unsafe hybrid generated forms like `promptت`
- inconsistent terminology

## Design checks

- missing page index → MAJOR
- random semantic type-role drift → MAJOR
- random font drift → MAJOR
- default Persian alignment drift without rationale → MAJOR
- 2+ semantic regions without grouping/override → MAJOR
- unexplained top dead-space band → MAJOR
- confusing primary visual → MAJOR
- decorative noise that competes with the message → MAJOR

## Brand / diversity checks

- wrong final footer domain → BLOCKER
- ASDEV overpowering content → revise
- category treated as fixed template → MAJOR
- same dominant palette/layout/image-treatment repeated without semantic reason when recent evidence exists → revise
- recent history fabricated → BLOCKER

## Render semantics

A written Art Direction PASS does not prove the rendered artifact is good.

Rendered previews require `rendered-preview-gate.md`.
Final production requires `final-render-verification.md`.
