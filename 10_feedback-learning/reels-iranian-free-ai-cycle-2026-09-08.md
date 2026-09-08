# Iranian Free AI Reel — Production Cycle — 2026-09-08

## Status

`APPROVED-RENDER`

User explicitly confirmed the final Google Flow render as: «واقعاً عالیه».

This document records the production decisions and the most important new learning from the Reel about Iranian AI tools so the successful behavior can be reused without repeating the failed robotic iteration.

---

## 1. Topic / Goal

Topic:

`هوش مصنوعی‌های برتر ایرانی`

Goal:

- introduce Iranian AI tools/services useful for everyday tasks;
- frame the tools as having free usage where applicable;
- keep the spoken Reel general and curiosity-driven;
- use a one-keyword CTA for receiving the names/details later.

CTA keyword:

`ایرانی`

Important claim rule:

Any future reuse of claims such as `رایگان`, free tier, free credits, availability inside Iran, registration requirements, usage caps, or pricing must be reverified before publication because product conditions can change.

---

## 2. Final Locked Dialogue — APPROVED RENDER

```text
«هوش مصنوعی‌های برتر ایرانی که می‌تونی برای کارهای روزمره به‌صورت رایگان استفاده کنی.

اگه اسمشون رو می‌خوای، کلمه ایرانی رو بفرست.»
```

### Dialogue decisions

Earlier three-block copy was rejected in practice because the generated delivery felt too mechanical and consecutive.

The final script was intentionally converted to:

1. one flowing primary statement;
2. one natural conversational beat;
3. one CTA.

The CTA remains a single keyword: `ایرانی`.

---

## 3. Visual Direction — APPROVED

Character direction:

- fictional original adult Iranian woman, mid-20s;
- contemporary Iranian creator appearance;
- soft beige / dusty-pink headscarf;
- stylish rounded eyeglasses;
- oversized light-blue denim jacket;
- simple black outfit underneath;
- understated wristwatch;
- natural realistic skin;
- fashionable, modest, youthful, creator-native styling;
- not a presenter and not a commercial fashion model.

Environment:

- stylish contemporary urban café with a modern Tehran-café feeling;
- large windows;
- softly blurred city architecture;
- warm spherical pendant lights;
- soft daylight mixed with warm café light;
- light café sofa + wooden table;
- optional natural table props such as pink drink, dessert, smartphone, laptop;
- no readable text, fake UI, generated subtitles, or logos.

Camera:

- vertical 9:16;
- 10 seconds;
- medium-close / upper-waist framing;
- eye level;
- one uninterrupted take;
- essentially locked camera;
- no cuts, transitions, orbit, dramatic zoom, or scene reset.

---

## 4. Failed Iteration — Robotic / Back-to-Back Delivery

### Symptom

User feedback:

`خیلی ماشینی و پشت سر هم میگه`

The earlier prompt used strongly engineered timing blocks and explicit per-block timing. Although the intent was to preserve silence, the result felt scheduled rather than human.

### Root cause

Over-specifying exact timestamps + multiple separated dialogue blocks + many simultaneous speech constraints can cause Flow to optimize for schedule compliance instead of natural acting.

This is an important refinement to older Absolute Audio Timeline guidance.

### Corrective decision

Do NOT assume exact timestamps are always the best solution.

When the render becomes robotic:

- simplify the dialogue architecture first;
- remove unnecessary exact second-by-second choreography;
- preserve only the important conversational beat;
- explicitly prioritize natural human delivery over timestamp compliance;
- allow breathing and micro-pauses inside a sentence;
- allow facial reactions to emerge semantically;
- never solve timing by making speech faster.

---

## 5. New Promoted Learning — Semantic Conversational Beats

The successful render used a natural performance contract rather than an absolute audio timeline.

Key contract:

```text
The performance must feel like a real young Iranian woman casually talking to her audience in one natural take.

Do NOT make the speech sound timed, programmed, robotic, rehearsed, or like a commercial.

HIGH ENERGY DOES NOT MEAN FAST SPEECH.

Allow natural breathing.
Allow natural micro-pauses inside the sentence.
The speaker does NOT need to say the entire first sentence in one continuous breath.

Facial expressions must emerge naturally from the meaning of the sentence.
Do not choreograph gestures for individual words.
Do not pose after each sentence.
Do not reset the face between speech blocks.

After the main statement, allow a real conversational beat before the CTA.
The speaker must not freeze during the beat.

Natural human delivery is more important than exact second-by-second timing.
If necessary, reduce empty lead-in/end time rather than accelerating speech.
```

### Promotion rule

Use **Absolute Audio Timeline** when Flow collapses required pauses or begins blocks prematurely.

Use **Semantic Conversational Beats** when exact timing itself causes robotic, scheduled, presenter-like delivery.

These are now two different corrective tools, not one universal rule.

---

## 6. Facial / Body Performance — APPROVED BEHAVIOR

Successful direction:

```text
Natural spontaneous Iranian creator energy.
Confident, friendly, slightly excited.
Natural breathing.
Natural micro-pauses.
Natural spontaneous body language.
Small unscripted hand movement is allowed.
Natural head movement is allowed.
Natural weight shift is allowed.
Expressions emerge from sentence meaning.
```

Avoid:

- gesture per keyword;
- deliberate eyebrow cue on every important word;
- repeated nodding;
- exaggerated pointing;
- artificial facial-expression reset;
- freeze during pauses;
- presenter/commercial delivery.

This reinforces GFVPN-002 and adds evidence from an explicitly approved final render.

---

## 7. Clean Raw Camera Contract

The prompt retained the successful clean-camera direction:

```text
The result must look like raw camera footage from a real creator recording in a café.

No subtitles.
No captions.
No automatic transcription.
No Persian text.
No English text.
No graphics.
No stickers.
No floating words.
No arrows.
No logos.
No buttons.
No fake social-media interface.
No fake browser.
No UI overlay.
```

No generated text should be trusted for the final asset; any desired typography belongs in editing/cover production.

---

## 8. Reference / Character Rule

The visual direction was expressed self-contained in the production prompt rather than depending on a person reference.

Keep the character:

- entirely fictional;
- original;
- adult;
- self-contained through generic visual attributes.

Do not attempt to recreate a real/public/recognizable person.

---

## 9. Approved Production Pattern from This Cycle

For a short 10-second Iranian-Persian creator Reel with one main claim + CTA:

```text
TOPIC / HOOK
→ one naturally flowing benefit statement
→ natural conversational beat
→ one short CTA
→ silent/natural end
```

Performance priority:

```text
human rhythm
> facial semantic reaction
> natural breathing
> exact timestamp compliance
```

Timing constraint should be added only as strongly as the observed failure requires.

---

## 10. Evidence / User Approval

Final generated file supplied by user in conversation:

`irani.mp4`

User verdict:

`پرامپت و دادم و ویدیویی که ساخت واقعا عالیه`

Therefore the final dialogue + natural-performance prompt direction are promoted to `APPROVED-RENDER` evidence for future Reel production.

The binary video itself is not committed to this documentation repository in this update; the approval and production provenance are recorded here.

---

## 11. Next Workflow Gate

Current state:

- [x] Direction approved
- [x] Script approved
- [x] Character / environment approved
- [x] Google Flow prompt rendered
- [x] Render QA by user: PASS
- [x] Production learning recorded
- [ ] Cover direction
- [ ] Cover
- [ ] Caption / publish pack
- [ ] Publish
- [ ] Post-publish metrics / learning

Do not mark this Reel `PUBLISHED` until publication is explicitly confirmed.
