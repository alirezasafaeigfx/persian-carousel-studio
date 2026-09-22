# ASDEV Story Engine — Design Spec

Date: 2026-09-17
Last updated: 2026-09-22
Status: Pilot active — live evidence incorporated
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

Default test cadence for Story-native days:

- Wave 1: around 10:00 Tehran time
- Wave 2: around 12:30 Tehran time
- Wave 3: around 18:00 Tehran time

These remain test windows, not permanent rules.

### Reel-test exception

When the goal is to measure whether a Trial Reel can earn recommendation distribution on its own, do **not** immediately push it through Stories.

Use two phases:

1. **Organic isolation phase:** publish the Reel and capture an initial checkpoint before Story support. As a pilot default, leave a 3–6 hour Story-free window unless the owner intentionally wants immediate traffic or the Reel is already in obvious acceleration.
2. **Story boost phase:** reshare the Reel once with one clear curiosity/value CTA, then capture the same metrics again.

The 3–6 hour window is an experiment parameter, not a proven optimal posting rule.

## 6. Seven-day pilot — V2

The original pilot intent is retained, but the order is updated using live Story/Reel evidence from 2026-09-22.

### Day 1 — Curiosity-native Story

Goal:

- maximize Story continuation and replies without depending on a Reel reshare;
- test one curiosity hook against one clear useful payoff.

Sequence:

1. short curiosity hook;
2. one poll;
3. one proof/value frame;
4. one conversation frame.

### Day 2 — Free-tool utility test

Start from one broad pain. Show a genuinely free/useful capability, prove it with a screenshot or demo, then ask one low-friction question such as whether viewers want the tutorial or an alternative.

### Day 3 — Audience demand discovery

Use one poll or question sticker to identify the next high-demand AI category. Do not stack multiple research questions in the same frame.

### Day 4 — Human / behind-the-scenes

Show testing, failed attempts, prompt comparison, editing, or decision-making. Goal: relationship and trust, not direct conversion.

### Day 5 — Fast education

Use 3–4 frames:

`Hook -> one instruction -> proof/demo -> one follow-up question`

No filler frame.

### Day 6 — Controlled Story-to-Reel bridge

1. publish the Trial Reel;
2. capture the initial Reel checkpoint before Story support;
3. keep the Reel Story-free for the pilot isolation window when clean measurement is the goal;
4. reshare once in Story with one clear bridge CTA;
5. compare before/after source mix, follower mix, watch time, shares, comments and follows.

### Day 7 — Community review

Recap the strongest Story signal from the week, show one useful takeaway, and ask the audience to choose the next priority.

## 7. Current executable sequence — record-Story follow-up

Context: the Story attached to the current `+18 / free AI` Reel reached **2,154 Story viewers** in the screenshot supplied on 2026-09-22. The owner reported this as the highest Story view count seen on the page so far.

This is evidence for a follow-up test, not a permanent `+18` rule.

### Story 1 — Proof-led hook

Text:

`این استوری تا الان رکورد ویوی پیج رو زده 👀`

Secondary line:

`۲۱۵۴ نفر دیدنش.`

Job: proof + curiosity.

### Story 2 — Hypothesis poll

Text:

`فکر می‌کنی چی باعث شد بیشتر دیده بشه؟`

Poll direction:

- کنجکاوی «۱۸»
- ابزار رایگان

Job: collect audience perception; not scientific attribution.

### Story 3 — Transparent interpretation

Text:

`احتمالاً ترکیبِ کنجکاوی + یه ابزار کاربردی جواب داده؛ ولی با یه استوری نمی‌شه قطعی گفت.`

Job: maintain trust and explain that the page is testing, not pretending certainty.

### Story 4 — Demand capture

Text:

`تست بعدی رو روی چی انجام بدیم؟`

Question sticker:

`چه هوش مصنوعی رایگانی لازم داری؟`

Examples:

`عکس — ویدیو — درس — کار — سایت`

Job: turn the high-reach Story into research for the next content cycle.

## 8. Live evidence update — 2026-09-22

### Story evidence

Observed from owner-supplied Insights screenshot:

- Story viewers: **2,154**
- Reshares: **1**
- direct Story replies were present; the screenshot did not expose the full reply count
- owner report: this was the highest Story view count seen on the page so far

### Reel evidence at the same latest checkpoint

Observed from owner-supplied Reel Insights screenshots:

- Views: **3,963**
- Viewers: **2,705**
- Average watch time: **6s**
- Follows: **18**
- Likes: **31**
- Comments: **168**
- Reposts: **6**
- Shares: **107**
- Saves: **23**

Rate labels shown by Instagram:

- Skip rate: **50.3% — Lower**
- Share rate: **3.7% — Higher**
- Like rate: **1.1% — Lower**
- Save rate: **0.8% — Lower**
- Repost rate: **0.2% — Higher**
- Comment rate: **5.8% — Lower**

Top view sources:

- Stories: **68.3%**
- Reels tab: **16.7%**
- Explore: **3.2%**
- Profile: **2.0%**
- Search: **0.1%**

Audience mix:

- Followers: **70.9%**
- Non-followers: **29.1%**

### Scoped interpretation

The current evidence supports these working hypotheses:

1. **Stories can be a strong follower-reach and conversation engine for ASDEV.** The 2,154-view Story is meaningful page-level evidence, especially because the owner reports it as a record.
2. **Story success and Reel discovery are different jobs.** At the latest checkpoint, Stories supplied 68.3% of Reel views while Reels tab + Explore supplied a much smaller share. Therefore Story-driven views must not be treated as proof that the Reel itself is winning recommendation distribution.
3. **Story boosting can contaminate Reel experiments.** If the objective is to learn whether a Trial Reel can travel to non-followers organically, capture a clean pre-Story baseline first.
4. **The `18` curiosity mechanic is a candidate Story hook, not a permanent identity.** It produced strong curiosity in this cycle, but one success is insufficient to make it a default. Use it sparingly and pair it with a fast, honest utility payoff.
5. **Story replies are valuable research data.** When a high-reach Story generates direct replies, the next Story should convert that attention into one useful audience-demand question rather than immediately stacking another promotional CTA.

### Story-to-Reel Bridge Protocol V2

For future Trial Reels:

**Checkpoint A — before Story support**

Record:

- views / viewers;
- average watch time;
- skip rate;
- shares / comments / saves / follows;
- top sources;
- follower vs non-follower mix.

**Checkpoint B — after one Story bridge**

Reshare the Reel once with one clear reason to tap or reply. Do not combine multiple CTAs.

Then record the same metrics again.

**Checkpoint C — 24h review**

Classify:

- `REEL-LED` — recommendation sources and non-follower share expand independently;
- `STORY-ASSISTED` — meaningful growth occurs mainly after Story support;
- `STORY-WINNER / REEL-WEAK` — Story performs strongly but Reel discovery remains limited;
- `MIXED` — insufficient separation to infer direction.

These labels are operational classifications, not algorithmic claims.

## 9. Measurement model

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

## 10. Learning and promotion rules

Use the existing feedback-learning protocol.

A Story pattern becomes durable only when supported by one of:

- explicit durable owner instruction;
- repeated reinforcement across independent Story cycles;
- reinforcement of an existing quality/safety requirement.

One successful Story is evidence, not a permanent rule.

## 11. Planned repository structure after spec approval

Proposed additions:

- `15_stories/story-operating-system.md`
- `15_stories/story-narrative-system.md`
- `15_stories/story-format-library.md`
- `15_stories/story-hook-library.md`
- `15_stories/story-performance-ledger.md`
- `15_stories/story-7-day-pilot.md`

Implementation of the full `15_stories/` structure remains gated, but the pilot itself is now active and this spec has been updated with live evidence.

## 12. Non-goals

Not part of this phase:

- fully automated Story publishing;
- automatic DM funnels;
- automated AI-generated replies;
- fixed permanent timing rules;
- aggressive link-heavy conversion flows;
- turning every Reel into a mandatory Story sequence.

## 13. Review gate

Before implementation, verify:

- no TBD/TODO placeholders;
- no contradiction between Story sequence and CTA rules;
- the current executable sequence reflects the latest live Story evidence;
- measurement is based on observable Instagram/Metricool data;
- the system remains flexible enough to react to live audience feedback.
