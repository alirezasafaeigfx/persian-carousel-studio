# Carousel Foundation Tokens

These tokens are locked **inside one carousel**, not globally between different posts.

## Canvas

Standard Instagram carousel:

- Canvas: `1080 × 1350`
- Ratio: `4:5`
- Grid: `12 columns`
- Outer margins: `72px`
- Gutters: `24px`
- Base spacing unit: `12px`

## Semantic Type Scale

Before render choose exact values for this carousel and lock them:

- `T1` — Cover Display
- `T2` — Slide Headline
- `T3` — Key Statement / Subhead
- `T4` — Body
- `T5` — Caption / Microcopy
- `T6` — Source / Metadata / Page Index

Recommended working ranges:

- T1: ~104–124px
- T2: ~72–88px
- T3: ~52–64px
- T4: ~38–46px
- T5: ~28–34px
- T6: ~24–28px

Once exact values are selected, unexplained role drift greater than about `±4px` is a defect.

Use at most two font families unless explicitly justified.

## Page index

Required on every slide.

Choose once per carousel:

- format: e.g. `1/7` or `01/07`
- slot: `top-left` or `top-right`

Keep both fixed across the set.

Missing/inconsistent index = `MAJOR`.

## RTL anchor

Default Persian headline/body = right-aligned and anchored to the grid unless an explicit composition override is documented.

## Palette roles

Resolve semantic roles, not merely favorite colors:

- `BG`
- `INK`
- `ACCENT-1`
- optional `ACCENT-2`
- `MUTED`
- `LINE/BORDER`

Color role meaning must stay stable within the carousel.

## Spacing

Spacing must come from the 12px rhythm. Avoid freehand random gaps.

## Top-space gate

For ordinary layouts, primary content should usually enter composition by roughly `y ≤ 270px`.

A large blank top band after the header/navigation region needs a clear compositional function. Unexplained dead space is `REVISE/MAJOR` depending on severity.

## Components

If cards/frames/components are used, lock their padding/radius/stroke behavior for the set. Component use is optional; consistency is not.
