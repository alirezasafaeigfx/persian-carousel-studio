# Render Foundation Prompt Contract

Every image-generation prompt for a carousel slide must carry the resolved production constraints explicitly.

Words like `premium`, `modern`, `editorial`, `clean` are not substitutes for a foundation.

## Required prompt payload

```text
CANVAS:
- 1080×1350 / 4:5 unless explicitly overridden

GRID:
- 12 columns
- 72px margins
- 24px gutters

PAGE INDEX:
- exact format
- exact fixed slot

RTL:
- Persian anchor behavior

TYPE ROLES:
- exact locked T1–T6 values needed by this slide

PALETTE ROLES:
- BG / INK / ACCENT / MUTED / LINE

TOP SPACE:
- planned behavior / override if any

SEMANTIC REGIONS:
- region list
- grouping mechanism
- framing strength

BIDI PLAN:
- separate RTL and LTR visual elements
- punctuation ownership
- token order

VISUAL SEMANTIC MAP:
- what each primary visual represents

FOOTER:
- exact final behavior when producing final frame
```

## Mixed-script rule

Do not pass a critical mixed string such as `۳) OPTIONS: فقط یک جواب نخواه` as one generative text run.

Split it into separately placed elements.

## Exact text authority

When the generation system is unreliable for Persian typography, treat generated text as preview-only and preserve final copy for deterministic exact/hybrid rendering.
