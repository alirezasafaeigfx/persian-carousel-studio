# Rendered Preview Gate

This gate runs on the **actual rendered images** before they are shown as candidate previews.

## Per-slide checks

### Canvas / navigation

- correct 4:5 geometry or requested canvas;
- page index exists;
- page index format/slot is consistent.

### Typography

- T-role hierarchy matches locked foundation;
- font family/weight behavior is consistent;
- same semantic roles do not randomly change scale;
- headline is recognizable at mobile size.

### Alignment / spacing

- Persian anchor follows RTL plan;
- elements connect to grid/optical axes;
- top whitespace is purposeful;
- section gaps follow spacing rhythm.

### Semantic regions

For slides with 2+ major regions:

- visible grouping exists, or
- documented open-composition behavior is actually legible.

Unframed floating multi-region composition = `MAJOR`.

### Bidi

Inspect visible order of:

- Latin/code tokens;
- punctuation;
- Persian numbers/step badges;
- Persian headline/body around LTR tokens.

Broken mixed-direction order = `MAJOR`.

### Visual comprehension — 3 second test

Can a viewer understand what the main visual represents in about three seconds without reading a paragraph just to decode the image?

If no: simplify, annotate, replace or remove.

### Copy integrity

Generated Persian preview text is not authoritative final copy. Obvious broken text still makes a preview candidate unacceptable when it harms review of direction.

## Gate behavior

If any slide contains a MAJOR design-foundation / semantic-region / bidi / comprehension defect:

- revise/regenerate it;
- do not present that weak artifact as the candidate set.

Result:

`PASS | REVISE | INCOMPLETE`
