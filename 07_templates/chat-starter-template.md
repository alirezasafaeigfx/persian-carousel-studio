# Chat Starter Template

این template برای شروع هر chat جدید Persian Carousel Studio در ChatGPT است. وظیفهٔ آن **orchestration + selective reference routing** است؛ قوانین واقعی در GitHub می‌مانند.

Repository:

`https://github.com/alirezasafaeigfx/persian-carousel-studio`

## 1. Task Modes

- `full-carousel`
- `copy-only`
- `visual-only`
- `preview-only`
- `audit-only`
- `final-render-audit`
- `feedback-capture`

اگر پست کامل خواسته شد و mode مشخص نیست → `full-carousel`.

## 2. Run Modes

- `staged` — concept + Level A + Narrative Gate، سپس توقف برای approval.
- `auto` — direction انتخاب و workflow تا QA ادامه می‌یابد.

Default: `staged`.

## 3. Reference Modes

- `standard` — حداقل references لازم.
- `identity-aware` — visual identity/variation references را در art direction اضافه کن.
- `gold-assisted` — registry + حداکثر 2 Gold Standard مرتبط؛ surface detail را copy نکن.

## 4. Baseline Full-Carousel References

ابتدا فقط این‌ها:

- `01_brand/brand-voice.md`
- `02_persian-language/persian-style-guide.md`
- `03_content-system/carousel-narrative-system.md`
- `04_design-system/visual-design-system.md`
- `05_quality-control/anti-ai-qa.md`
- `07_templates/carousel-output-schema.md`

سپس brief را resolve کن؛ همهٔ completion files را از ابتدا load نکن.

## 5. Selective Routing

### Brand

در final/brand-sensitive tasks در صورت نیاز:

- `01_brand/brand-core.md`
- `01_brand/brand-signature.md`

`brand-architecture.md` فقط برای identity/routing conflict.

### Category / visual identity

- `12_marketing/content-category-system.md`
- برای art direction: `09_brand-identity/category-art-direction-system.md`
- `09_brand-identity/visual-variation-router.md`

### Marketing

- `12_marketing/marketing-objective-system.md`
- funnel/CTA modules فقط در صورت نیاز.

### Copy

- `13_copywriting/instagram-copywriting-system.md`
- hook حساس → `hook-headline-system.md`
- numeric/ranking/marketing claim → `persuasion-and-claim-discipline.md`
- CTA wording → `cta-copy-system.md`

### Recent-style exclusion

وقتی recent evidence واقعاً لازم است:

- `09_brand-identity/recent-style-exclusion.md`
- و فقط warm-memory index: `14_observations/recent-post-index.md`

برای این کار individual OBSها را load نکن.

اگر index خالی/ناکافی است:

`Recent-style conflict: unavailable`

history را حدس نزن.

### Design Foundation — REQUIRED BEFORE ANY VISUAL RENDER

حتماً load کن:

- `04_design-system/carousel-foundation-tokens.md`
- `04_design-system/semantic-region-bidi-contract.md`

Resolve and lock:

- `DESIGN FOUNDATION`
- `REGION GRAMMAR`
- `BIDI PLAN` برای mixed slides

بدون این‌ها: `Visual Production = INCOMPLETE`.

### Preview / image generation

اگر preview/render خواسته شد:

- `06_workflows/preview-to-final-workflow.md`
- `05_quality-control/rendered-preview-gate.md`
- `11_prompt-libraries/render-foundation-prompt-contract.md`
- بخش لازم از `11_prompt-libraries/image-prompt-library.md`

بعد از render و قبل از ارائهٔ candidate، Rendered Preview Gate را روی خود تصاویر اجرا کن. MAJOR defect → revise/regenerate.

## 6. Locked ASDEV Defaults

مگر user صریحاً خلافش را بخواهد:

- Brand: `ASDEV`
- Canvas: `4:5`
- Target: `1080 × 1350`
- Footer final: `alirezasafaeisystems.ir`
- Tone: `Friendly-natural`
- Colloquiality: `3`

در هر carousel foundation داخل همان set قفل می‌شود؛ palette/font/layout/image treatment بین پست‌ها قفل نیستند.

## 7. Mandatory Workflow

تا Narrative approval:

`Brief → Category → Marketing Job → Semantic Frame → 3+ Concept Directions → Direction Selection → Level A → Narrative Gate`

بعد از approval:

`Exact Persian Copy → Copy/Claim Audit → Visual Route → DESIGN FOUNDATION + REGION GRAMMAR + BIDI PLAN → Art Direction → Visual Gate → Level B → Anti-AI QA`

اگر preview:

`Foundation/Region/Bidi-Aware Prompt → Render → Rendered Preview Gate → regenerate until PASS → User Direction Review`

اگر final:

`Exact/Hybrid Final Production → Final Render Verification → production-ready`

## 8. Hard Rules

- unsupported numeric claim → BLOCKER
- fake fact/source/metric → BLOCKER
- generated broken Persian treated as final → BLOCKER
- wrong footer → BLOCKER
- missing page index → MAJOR
- random T-role/font/alignment drift → MAJOR
- multi-region slide without grouping/override → MAJOR
- broken RTL/LTR token order → MAJOR preview / BLOCKER final when meaning breaks
- unsafe hybrid generated word → MAJOR
- unexplained top dead space → MAJOR
- confusing primary visual → MAJOR
- whole-repo loading ممنوع

## 9. Daily Starter

```text
@GitHub
Source of Truth: https://github.com/alirezasafaeigfx/persian-carousel-studio

طبق 07_templates/chat-starter-template.md کار کن.
TASK MODE: full-carousel
RUN MODE: staged
REFERENCE MODE: identity-aware

موضوع پست:
[موضوع]
```

## 10. Production Observation Handoff

فقط بعد از outcome معنادار:

- accepted؛
- revise/reject با defect قابل نگهداری؛
- regression واقعی؛
- performance data صریح user.

اگر GitHub write access موجود است:

1. `14_observations/post-observation-template.md` را بخوان؛
2. `OBS-NNN-<slug>.md` را compact ثبت کن؛
3. فقط accepted/revise را وارد rolling `recent-post-index.md` کن؛
4. durable preference را فقط از مسیر Feedback Ledger promote کن؛
5. regression فقط اگر reproducible/systemic است؛
6. Gold Standard فقط scoped.

Cold path در normal generation:

- individual `14_observations/posts/*`
- synthesis history
- regression history
- governance/acceptance docs

Checkpoint:

- 10 observations → SYN-010
- 20 observations → SYN-020
