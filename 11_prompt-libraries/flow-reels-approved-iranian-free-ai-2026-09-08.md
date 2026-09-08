# Flow Reels — Iranian Free AI — Approved Prompt Baseline — 2026-09-08

## Status vocabulary

- `APPROVED-RENDER` — final generated output explicitly approved by user.
- `APPROVED-PATTERN` — reusable prompt component supported by approved output.
- `CORRECTIVE-PATTERN` — response to an observed failure.

---

# IRFAI-001 — Final Locked Dialogue

**Status:** `APPROVED-RENDER`

```text
«هوش مصنوعی‌های برتر ایرانی که می‌تونی برای کارهای روزمره به‌صورت رایگان استفاده کنی.

اگه اسمشون رو می‌خوای، کلمه ایرانی رو بفرست.»
```

CTA keyword: `ایرانی`

Mutable claim warning: before publishing/reusing this concept, reverify free-tier/free-credit/access conditions for the actual Iranian services being recommended.

---

# IRFAI-002 — Natural Conversational Performance Contract

**Status:** `APPROVED-RENDER + APPROVED-PATTERN`

This pattern corrected a robotic/back-to-back Flow render caused by over-engineered exact timing.

```text
The performance must feel like a real young Iranian woman casually talking to her audience in one natural take.

Do NOT make the speech sound timed, programmed, robotic, rehearsed, or like a commercial.

Natural spontaneous Iranian creator energy.
Confident, friendly, slightly excited.

HIGH ENERGY DOES NOT MEAN FAST SPEECH.

Allow natural breathing.
Allow natural micro-pauses inside the sentence.
She does NOT need to say the entire first sentence in one continuous breath.

Her face must react naturally to what she is saying.
Expressions should emerge naturally from sentence meaning.

After finishing the main statement, allow a brief real conversational beat.
Her lips close naturally.
She keeps eye contact.
A tiny spontaneous facial reaction, subtle breath, or expression change may happen.
She must NOT freeze.
She must NOT pose.
She must NOT reset her face.

Then deliver the CTA naturally, almost like giving the viewer the next step.

Natural human delivery is more important than exact second-by-second timing.
The entire dialogue should comfortably fit within the clip while preserving natural rhythm, breathing and facial reactions.
If necessary, reduce empty time at the beginning or end.
DO NOT solve timing by making her speak unnaturally fast.
```

---

# IRFAI-003 — Body Language Contract

**Status:** `APPROVED-PATTERN`

```text
Natural spontaneous body language only.
Small unscripted hand movement is allowed.
Natural head movement is allowed.
Natural weight shift is allowed.

Do NOT assign a gesture to individual words.
No pointing at invisible text.
No repeated nodding.
No repeated eyebrow movements.
No exaggerated hand gestures.
No presenter choreography.
The body should never return to a fixed pose after each phrase.
```

This strengthens the earlier GFVPN-002 natural-acting pattern with explicit approved-render evidence.

---

# IRFAI-004 — Visual Baseline

**Status:** `APPROVED-RENDER-DIRECTION`

```text
Entirely fictional original Iranian adult woman, mid-20s.
Contemporary Iranian appearance.
Soft beige / dusty-pink headscarf naturally wrapped around head and neck.
Stylish rounded eyeglasses.
Oversized light-blue denim jacket.
Simple black outfit underneath.
Minimal wristwatch.
Natural realistic skin.
Fashionable, modest, youthful, creator-native.
Not a television presenter.
Not an advertising model.

Stylish modern urban café with contemporary Tehran-café feeling.
Large windows.
Soft daylight.
Warm spherical pendant lights.
Modern interior.
Light café sofa.
Wooden table.
Optional pink drink, dessert, smartphone and laptop as natural physical props.
```

---

# IRFAI-005 — Camera / Continuity

**Status:** `APPROVED-PATTERN`

```text
Vertical 9:16.
10 seconds.
Medium-close framing.
Eye-level camera.
One single uninterrupted recording.
Camera remains essentially locked and stable.

No cuts.
No transitions.
No scene changes.
No dramatic zoom.
No orbit.
No cinematic camera movement.

Same woman, face, headscarf, glasses, clothing, lighting, café, objects, camera and lens throughout.
No visual resets.
```

---

# IRFAI-006 — Clean Raw Camera

**Status:** `APPROVED-PATTERN`

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

Every visible element must physically belong to the real café scene.
```

---

# IRFAI-007 — Timing Strategy Selector

**Status:** `CORRECTIVE-PATTERN`

Do not treat exact timestamps as universal.

### If Flow collapses pauses / starts blocks early

Use the existing Absolute Audio Timeline / Speech-Silence contract.

### If Flow sounds robotic because it is following the timeline too literally

Use IRFAI-002 Natural Conversational Performance Contract:

- remove unnecessary exact timestamps;
- simplify speech into one main statement + CTA;
- preserve a semantic conversational beat;
- allow natural micro-pauses and breathing;
- prioritize human rhythm over timestamp precision.

Rule:

`Use the minimum timing constraint necessary to fix the observed failure.`

---

# IRFAI-008 — Final Success Test

**Status:** `APPROVED-PATTERN`

```text
The result should feel like a real Iranian creator sitting casually in a stylish café, naturally sharing a useful discovery with her audience, taking small human breaths and conversational beats, reacting naturally with her face, then casually asking viewers to send the word «ایرانی».

It must NOT feel scripted, mechanical, timed, commercial, presenter-like or machine-gun fast.
```

---

# Approval Evidence

User rendered the final prompt in Google Flow and supplied `irani.mp4`.

Explicit verdict:

`پرامپت و دادم و ویدیویی که ساخت واقعا عالیه`

Therefore IRFAI-001 and IRFAI-002 are considered approved-render evidence, not merely theoretical prompt directions.
