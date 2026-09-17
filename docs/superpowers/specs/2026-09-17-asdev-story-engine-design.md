# ASDEV Story Engine — Design Spec

Date: 2026-09-17
Status: Draft for owner review
Scope: Instagram Stories operating system for ASDEV

## 1. Purpose

Turn Instagram Stories from ad-hoc support content into a measurable growth and audience-research system that complements Reels and carousels.

Primary goals:

- raise the floor of Story reach and interaction;
- use Stories to reactivate strong Reels;
- discover audience demand before producing new Reels;
- create a repeatable feedback loop across Stories, Reels and carousel content;
- record only evidence-backed learnings as durable rules.

## 2. Strategic model

Chosen model: **Hybrid Story Engine**.

Why:

- fixed structure prevents random posting;
- flexible slots allow reaction to live performance, audience answers and new opportunities;
- avoids overfitting one successful Story into a permanent rule.

Content balance for the pilot:

- ~70% education, useful tools and practical value;
- ~30% behind-the-scenes, opinion, testing and human interaction.

## 3. Story sequence architecture

Default sequence:

`Hook -> Interaction -> Value -> Proof -> Conversation -> Reel Bridge / CTA`

This is a menu, not a mandatory six-frame checklist.

Rules:

1. Every Story frame must have one primary job.
2. Every frame must add information or trigger a distinct user action.
3. Remove filler frames created only to increase count.
4. The first frame should establish relevance immediately.
5. Proof must match the claim shown in the sequence.
6. CTA must be single-path and low-friction.
7. Avoid stacking follow + reply + link + comment requests in one sequence.

## 4. Format library

Supported formats:

- talking-head hook;
- poll;
- question sticker;
- screen recording;
- tool/demo proof;
- screenshot / social proof;
- behind-the-scenes process;
- Reel reshare / Reel bridge;
- audience answer follow-up;
- result reveal.

Talking-head characters such as Rose/Lia are used selectively for high-salience hooks, short explanations and key CTAs. They should not dominate every Story, so the feed remains creator-native rather than looking like a fully synthetic ad sequence.

## 5. Publishing cadence

Default test cadence for the pilot:

- Wave 1: around 10:00 Tehran time
- Wave 2: around 12:30 Tehran time
- Wave 3: around 18:00 Tehran time

These are test windows, not permanent rules. They should be retained, changed or retired only after enough live Story evidence exists.

## 6. Seven-day pilot

### Day 1 — Reactivate a strong Reel

Goal:

- return Story viewers to a high-performing Reel;
- collect direct audience experience;
- identify unmet demand for the next content cycle.

Sequence:

1. Talking-head curiosity hook.
2. Poll: whether the viewer already saw the Reel.
3. Social proof from the Reel performance.
4. Question sticker asking for real tool experience / limits.
5. Direct Reel reshare with one navigation CTA.
6. Question sticker asking what type of AI/tool the audience wants next.

### Day 2 — Audience demand discovery

Use Day 1 answers to identify one broad pain or desired tool category. Run a binary or 3-way poll, then follow with one useful mini-answer.

### Day 3 — Fast education

Short educational sequence around one concrete task. Use a hook, one instruction, one demo and one low-friction follow-up question.

### Day 4 — Free-tool utility test

Start from a broad pain. Show the free benefit, prove it with a live demo, then ask whether users want a deeper tutorial or an alternative.

### Day 5 — Human / behind-the-scenes

Show testing, failed attempts, decision-making or production process. Goal is trust and relationship, not conversion.

### Day 6 — Story-to-Reel bridge

Prime the audience before publishing or resurfacing a Reel. Measure how many Story viewers move into Reel interaction.

### Day 7 — Community review

Recap what won during the week, ask one clear question about next-week priorities, and record the strongest repeated signal.

## 7. Day 1 exact production plan

Context: use the currently strong AI Reel as the main asset.

### Story 1 — Hook

Format: Rose/Lia talking head, 5–7 seconds.

Dialogue:

«این ریلز یه اتفاق جالب براش افتاده... بیشتر کسایی که دیدنش اصلاً فالوورمون نبودن.»

On-screen support text:

`بیشتر بیننده‌ها فالوور نبودن!`

Job: curiosity + relevance.

### Story 2 — Poll

Format: 5–7 second excerpt from the Reel.

Text:

`تو اینو دیده بودی؟`

Poll options:

- آره، دیدمش
- نه، ندیده بودم

Job: estimate Story audience overlap with the Reel.

### Story 3 — Social proof

Format: clean Insights screenshot.

Text:

`این ویدیوی ۸ ثانیه‌ای تا الان بیشتر از ۱۵۰ نفر رو به پیج آورده.`

Secondary line:

`ولی چیزی که بیشتر برام جالبه، کامنت‌های شماست.`

Job: proof and transition toward conversation.

### Story 4 — Product feedback

Format: Reel/tool visual + question sticker.

Text:

`حالا کسایی که تستش کردین یه چیزو بگین 👇`

Question sticker:

`کجا محدودت کرد؟`

Alternative if needed:

`واقعاً بدون محدودیت بود؟`

Job: collect real usage evidence.

### Story 5 — Reel bridge

Format: native Reel reshare in Story.

Top text:

`اگه ندیدیش، این همونه 👆`

Bottom text:

`بعد از تست برگرد و نتیجه‌تو بهم بگو.`

Job: single-path navigation back to the Reel.

### Story 6 — Demand capture

Format: question sticker.

Text:

`اگه قرار باشه فردا یکی دیگه مثل این معرفی کنم...`

Sticker:

`دنبال چه هوش مصنوعی‌ای هستی؟`

Examples:

`عکس — ویدیو — درس — کار — سایت`

Job: generate candidate topics for the next Story/Reel cycle.

## 8. Measurement model

For every Story sequence, record:

- publish time;
- frame type;
- hook architecture;
- 24h views / reach;
- replies;
- poll votes;
- question-sticker responses;
- shares where available;
- exits / forward taps / back taps when available;
- qualitative user feedback;
- downstream Reel interaction when relevant.

Do not infer causal success from views alone.

### Pilot success questions

At the end of the 7-day pilot, answer:

1. Which hook architectures repeatedly hold reach?
2. Which interaction formats produce the highest response density?
3. Which time windows consistently perform better?
4. Which topics produce enough demand to justify Reel production?
5. Does Story-to-Reel bridging measurably increase Reel interaction?
6. Which behind-the-scenes formats improve replies without hurting continuation?

## 9. Learning and promotion rules

Use the existing feedback-learning protocol.

A Story pattern becomes durable only when supported by one of:

- explicit durable owner instruction;
- repeated reinforcement across independent Story cycles;
- reinforcement of an existing quality/safety requirement.

One successful Story is evidence, not a permanent rule.

## 10. Planned repository structure after spec approval

Proposed additions:

- `15_stories/story-operating-system.md`
- `15_stories/story-narrative-system.md`
- `15_stories/story-format-library.md`
- `15_stories/story-hook-library.md`
- `15_stories/story-performance-ledger.md`
- `15_stories/story-7-day-pilot.md`

Implementation begins only after owner review of this spec.

## 11. Non-goals

Not part of this phase:

- fully automated Story publishing;
- automatic DM funnels;
- automated AI-generated replies;
- fixed permanent timing rules;
- aggressive link-heavy conversion flows;
- turning every Reel into a mandatory Story sequence.

## 12. Review gate

Before implementation, verify:

- no TBD/TODO placeholders;
- no contradiction between Story sequence and CTA rules;
- Day 1 uses the approved strong Reel as the anchor asset;
- measurement is based on observable Instagram/Metricool data;
- the system remains flexible enough to react to live audience feedback.
