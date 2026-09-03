# Feedback Learning Protocol

این سند مشخص می‌کند Persian Carousel Studio چگونه از feedback کاربر **یاد می‌گیرد بدون اینکه بیش‌ازحد تعمیم دهد**.

هدف ساخت memory جادویی یا خودکار نیست. هدف این است که feedbackهای مهم با provenance در GitHub ثبت شوند و فقط در scope درست روی کارهای آینده اثر بگذارند.

## Core Principle

`Feedback → classify → scope → evidence → record → promote / keep local → supersede when needed`

هر feedback جدید را فوراً به قانون دائمی تبدیل نکن.

## Feedback Classes

### task-local

فقط برای task جاری معتبر است.

### candidate-preference

سیگنال واقعی وجود دارد، اما برای rule global کافی نیست.

### canonical-preference

ترجیح پایدار با evidence کافی.

### negative-rule

pattern پایداراً رد شده است.

### superseded

rule قبلی با evidence جدیدتر جایگزین شده است؛ history حذف نمی‌شود.

## Canonicalization Gate

Feedback فقط وقتی می‌تواند durable شود که حداقل یکی برقرار باشد:

### Gate A — Explicit Durable Language

مثل «از این به بعد»، «همیشه»، «برای همه پست‌ها».

### Gate B — Repeated Reinforcement

همان preference در حداقل 2 task مستقل صریحاً reinforce شده باشد.

### Gate C — Existing System Requirement

feedback یک quality/safety rule موجود را reinforce کند.

## What does not canonicalize automatically

- «عالیه»
- «خوبه»
- approval یک preview
- انتخاب یک option برای یک post
- سکوت کاربر
- performance حدس‌زده‌شده

## Scope principle

**Narrowest justified scope wins.**

نمونه scope:

- task-only
- topic-family
- preview-workflow
- final-production
- copy-style
- visual-hierarchy
- visual-identity
- all-carousels

## Confidence

`low | medium | high` فقط operational label است؛ confidence بالا broad scope را خودکار توجیه نمی‌کند.

## Ledger Schema

```text
ID:
Date:
Source task / pilot:
User feedback summary:
Evidence type:
Class:
Scope:
Confidence:
Interpreted rule:
Status: active | promoted | superseded | retired
Promoted to:
Supersedes:
Superseded by:
Notes:
```

## Promotion paths

- Gold Standard — scoped successful evidence
- Visual Identity Grammar — durable identity preference only
- Brand Voice / Persian Style — durable wording/tone behavior
- QA / Negative Rule — persistent failure pattern
- Workflow — durable process decision

## Performance feedback

Only explicit user-provided performance data may become performance evidence. Never invent reach, saves, engagement, conversion or causal results.

## Chat workflow

When feedback has future value:

1. apply it to the current task;
2. classify and scope it;
3. record compactly;
4. promote only if justified;
5. update only affected canonical references;
6. never rewrite the whole repo because of one feedback item.

## Canonicalization Principle

> **کمتر، دقیق‌تر و با provenance بهتر یاد بگیر.**
