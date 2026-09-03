# REG-001 — New-Chat Render Design Foundation

Status: `GREEN`

## Failure observed

A real fresh-chat seven-slide carousel produced artifacts with:

- missing page numbers;
- inconsistent typography hierarchy;
- inconsistent alignment;
- excessive empty top space;
- confusing visuals;
- written Art Direction marked PASS despite weak rendered execution.

## Root cause

The old design language named roles but did not enforce enough numeric/operational tokens at render time.

## Fix

- hard 4:5 foundation;
- numeric grid/margins/gutters/spacing rhythm;
- semantic `T1–T6` system;
- required page index;
- RTL anchor behavior;
- top-space gate;
- semantic visual comprehension check;
- foundation-aware prompt contract;
- Rendered Preview Gate before user presentation.

## Regression expectation

Missing page index, unexplained type/alignment drift, dead top space or confusing visual must no longer pass as a clean preview candidate.
