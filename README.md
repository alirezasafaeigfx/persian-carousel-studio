# Persian Carousel Studio

مرجع اصلی و نسخه‌پذیر برای طراحی و تولید حرفه‌ای پست‌های کاروسل فارسی ASDEV در ChatGPT.

> **Source of Truth:** `https://github.com/alirezasafaeigfx/persian-carousel-studio`

## Operating Model

این repository **Source of Truth** است. ChatGPT محیط اجراست و تاریخچهٔ یک chat مرجع دائمی نیست.

مدل استاندارد:

1. برای هر پست یک chat جدید.
2. از `07_templates/chat-starter-template.md` استفاده کن.
3. فقط referenceهای لازم همان task را بخوان.
4. GitHub rules از memory چت و preferenceهای استنباطی authoritativeتر هستند.

اصل مرکزی:

> **کمترین context لازم، با بیشترین وضوح تصمیم.**

## Locked ASDEV Defaults

برای standard Instagram carousel مگر user صریحاً خلافش را بخواهد:

- Brand mark: `ASDEV`
- Final footer: `alirezasafaeisystems.ir`
- Canvas: `4:5`
- Target production size: `1080 × 1350`
- Instagram tone: `Friendly-natural`
- Default colloquiality: `3`
- Page index روی همهٔ اسلایدها
- Persian-first / RTL-first composition

### Not globally locked between posts

- palette hue
- font family
- headline composition
- layout family
- card geometry
- motif
- image treatment
- illustration style
- framing primitive

> **Brand consistency ≠ visual repetition.**

## Canonical Runtime References

### Baseline full-carousel references

- `01_brand/brand-voice.md`
- `02_persian-language/persian-style-guide.md`
- `03_content-system/carousel-narrative-system.md`
- `04_design-system/visual-design-system.md`
- `05_quality-control/anti-ai-qa.md`
- `07_templates/carousel-output-schema.md`

همهٔ فایل‌های دیگر task-routed هستند. Whole-repo loading ممنوع است.

### Design / Render

- `04_design-system/carousel-foundation-tokens.md`
- `04_design-system/semantic-region-bidi-contract.md`
- `05_quality-control/rendered-preview-gate.md`
- `05_quality-control/final-render-verification.md`
- `06_workflows/preview-to-final-workflow.md`
- `11_prompt-libraries/render-foundation-prompt-contract.md`

### Intelligence / Identity

- `08_examples/gold-standard-registry.md`
- `09_brand-identity/visual-identity-grammar.md`
- `09_brand-identity/category-art-direction-system.md`
- `09_brand-identity/visual-variation-router.md`
- `09_brand-identity/recent-style-exclusion.md`
- `10_feedback-learning/feedback-learning-protocol.md`
- `10_feedback-learning/feedback-ledger.md`

### Marketing / Copy

- `12_marketing/content-category-system.md`
- `12_marketing/marketing-objective-system.md`
- `12_marketing/content-funnel.md`
- `12_marketing/cta-strategy.md`
- `13_copywriting/instagram-copywriting-system.md`
- `13_copywriting/hook-headline-system.md`
- `13_copywriting/persuasion-and-claim-discipline.md`
- `13_copywriting/cta-copy-system.md`

## Mandatory Full-Carousel Workflow

تا Narrative approval:

`Brief → Category → Marketing Job → Semantic Frame → 3+ Concepts → Selection → Level A → Narrative Gate`

بعد از approval:

`Exact Copy → Copy/Claim Audit → Visual Route → DESIGN FOUNDATION + REGION GRAMMAR + BIDI PLAN → Art Direction → Visual Gate → Level B → Anti-AI QA`

اگر preview:

`Foundation/Region/Bidi-Aware Prompt → Render → Rendered Preview Gate → Regenerate until PASS → User Direction Review`

اگر final:

`Exact/Hybrid Production → Final Render Verification → production-ready`

## Production Observation Memory

Evidence layer:

- `14_observations/README.md`
- `14_observations/post-observation-template.md`
- `14_observations/recent-post-index.md`
- `14_observations/posts/`
- `14_observations/synthesis/`

Memory tiers:

- **Hot:** baseline + task-routed canonical rules
- **Warm:** `recent-post-index.md` فقط وقتی recent-style evidence لازم است
- **Cold:** individual observations، synthesis، regressions، acceptance/governance history

Normal carousel generation نباید cold memory را load کند.

Learning loop:

`Build posts → observe compactly → synthesize at 10/20 → change architecture only with evidence`

## Current Status

- **Phase 1 — COMPLETE**
- **Phase 2 — COMPLETE**
- **Phase 3 — ACCEPTED / FROZEN**
- **Production Observation Memory — ACTIVE**
- **Phase 4 — DEFERRED / EVIDENCE-GATED**

## Migration / Restore Records

این repository نسخهٔ بازیابی‌شدهٔ baseline پذیرفته‌شده است.

- دلیل مهاجرت و محدودیت‌های تاریخچه: `MIGRATION.md`
- manifest بررسی سلامت baseline بازیابی‌شده: `RESTORE_INTEGRITY.md`

از این migration به بعد فقط همین repository authority دارد.
