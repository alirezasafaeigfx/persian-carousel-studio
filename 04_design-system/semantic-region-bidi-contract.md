# Semantic Region + Bidi Contract

## 1. Semantic Region Grammar

Grid tells elements where to sit. Region grammar tells the eye what belongs together.

If a slide has **2+ major semantic regions**, it needs visible grouping unless an `OPEN-COMPOSITION OVERRIDE` is documented.

Valid grouping mechanisms include:

- divider / rule;
- frame / partial frame;
- band / background field;
- split axis;
- rail / bracket;
- connected flow;
- annotated zone;
- contrast boundary;
- semantically justified cards.

Whitespace alone is not the default solution for example/comparison/process slides.

Do **not** turn every slide into the same card template.

### Framing strength

- `F0` — intentional open composition, override required for multi-region slides
- `F1` — light rule / rail / anchor
- `F2` — structured regions
- `F3` — comparison/data/component-dense framing

## 2. Direction-Safe Text Composition

Critical Persian + Latin/code content must not be delegated to one unsafe mixed-direction image text run.

Unsafe production instruction:

`۳) OPTIONS: فقط یک جواب نخواه`

Preferred decomposition:

- Persian step badge as its own element;
- `OPTIONS:` as an isolated LTR token;
- Persian headline as its own RTL element.

## 3. Bidi Plan

For every mixed-script slide define:

- which tokens are RTL;
- which tokens are isolated LTR;
- punctuation ownership;
- visual order;
- line-break behavior.

For exact final text use `dir=ltr` / `unicode-bidi:isolate` or equivalent isolation for LTR spans.

Broken token order = `MAJOR` preview and `BLOCKER` final when meaning changes.
