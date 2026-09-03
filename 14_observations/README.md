# Production Observation Memory

این پوشه حافظهٔ خارجی و evidence layer برای استفادهٔ واقعی Persian Carousel Studio است.

هدف آن آموزش وزن‌های مدل یا نگهداری transcript چت نیست. هدف این است که تجربهٔ واقعی تولید پست به evidence کوچک، قابل‌ردیابی و قابل‌تحلیل تبدیل شود تا سیستم فقط با شواهد واقعی تغییر کند.

## Core Loop

`Build post → meaningful production outcome → compact Observation → evidence classification → optional Ledger / Regression / Gold Standard promotion → SYN-010 / SYN-020 synthesis → canonical change only when governance allows`

Observation خودش rule نیست.

## Memory Tiers

### Hot Memory

فایل‌های canonical و task-routed موجود در workflow اصلی. Baseline full-carousel با این پوشه بزرگ نمی‌شود.

### Warm Memory

تنها فایل این پوشه که در کار عادی ممکن است selective load شود:

- `14_observations/recent-post-index.md`

فقط وقتی recent-style diversity/exclusion واقعاً به history اخیر نیاز دارد.

### Cold Memory

به‌صورت پیش‌فرض در ساخت carousel خوانده نمی‌شوند:

- `14_observations/posts/OBS-*.md`
- `14_observations/synthesis/*`
- historical observation details

## When to write

Observation فقط بعد از outcome معنادار:

1. preview/final explicitly accepted؛
2. meaningful revise/reject with reusable defect؛
3. real regression؛
4. explicit user-provided performance data.

Do not create for ordinary brainstorming or abandoned drafts.

## Never store

- private chain-of-thought / hidden reasoning;
- full chat transcript;
- large prompt dumps;
- invented metrics;
- irrelevant personal data.

## Relationship

- Observation = compact production evidence
- Feedback Ledger = durable/scoped preference
- Regression = reproducible/systemic contract failure
- Gold Standard = scoped successful reference evidence

Cross-reference IDs instead of duplicating long explanations.

## Synthesis

- Observation 10 → `SYN-010-production-review.md`
- Observation 20 → `SYN-020-learning-review.md`

Synthesis analyzes evidence; it does not automatically change architecture.

> **کمتر ثبت کن، دقیق ثبت کن، و فقط با evidence یاد بگیر.**
