# Secret Prompts Reel + Telegram PDF Funnel — Production Cycle — 2026-09-23

**Status:** `APPROVED-RENDER` + `APPROVED-FUNNEL-DIRECTION` + `PDF-READY`

This document records the full production cycle for the ASDEV Reel built around the concept **«پرامپت‌های سِرّی»**.

The goal is to preserve the successful render, the failed attempts, the corrective rules, the final distribution funnel and the reusable learnings so future Reels do not repeat the same trial-and-error.

---

## 1) Final locked Reel

### Approved video

- File: `P4.mp4`
- Duration: approximately **10.005 seconds**
- Resolution: **720×1280**
- Format: vertical 9:16
- Status: **APPROVED-RENDER**
- User decision: **freeze the video; no more regeneration**
- Character: Rose
- Genre: cinematic spy-thriller / secure-facility escape
- Spoken CTA keyword: **پرامپت**

Once `P4.mp4` was approved, the production moved forward to cover, captions, Telegram/PDF funnel and supporting assets.

---

## 2) Final locked Persian dialogue

The final spoken dialogue is immutable:

```text
«پرامپت‌های سِرّی که هیچ‌کس بهت نمیگه...

فقط بگو چی می‌خوای، خودش برات یه پرامپت دقیق می‌سازه.

میخوایش؟ پرامپت رو کامنت کن.»
```

### Important

After the final pronunciation passed, the user explicitly required that the dialogue remain unchanged while only action, movement and scene logic were refined.

Permanent scoped rule:

> Once Persian wording and pronunciation are approved in a Flow/Veo Reel, freeze the spoken script and make subsequent iterations visual-only unless the user explicitly reopens dialogue.

---

## 3) Concept and visual direction

The Reel concept is a secret / classified-prompt reveal.

Rose is escaping through an underground security corridor while sharing the prompt with the viewer.

Visual language:

- dark industrial corridor
- concrete + steel
- red emergency lighting
- security siren
- controlled handheld camera
- off-screen pursuit
- physical cover
- safe-room escape
- black tactical wardrobe
- magenta + sapphire Rose hair preserved
- no generated text in the video
- no visible weapon or shooter

The Reel should feel like a real spy-thriller moment, not a presenter video.

---

## 4) Key failures and fixes

### Failure A — flat robotic delivery

Early prompts over-constrained movement with phrases such as:

- restrained movement
- almost locked camera
- limited gestures
- do not overact
- do not turn this into action

The model responded by producing a calm talking-head performance with weak facial acting and body language.

### Fix

Action had to become part of the blocking itself:

- move toward cover
- react after gunfire
- physically hide behind concrete
- push away from cover
- accelerate toward safety
- enter safe room
- close door

Higher-order rule:

> If physical action matters, describe the action as required blocking, not as emotional adjectives.

---

### Failure B — pronunciation instability

Two risky words were removed from the spoken script after demonstrated failures:

- `محرمانه`
- `حرفه‌ای`

The final safer wording became:

- `سِرّی`
- `پرامپت دقیق`

This follows the existing lexical-rewrite rule already proven in earlier Flow cycles:

> When a token repeatedly mispronounces, prefer a safer lexical rewrite instead of adding increasingly complex phonetic instructions.

---

### Failure C — random left/right wall impacts

One render placed bullet impacts on both side walls late in the corridor.

This broke the physical story because the shooter was supposed to remain behind Rose.

### Root cause

The prompt described impacts without first enforcing one persistent line-of-fire topology.

### Fix

The scene geography was simplified:

```text
UNSEEN SHOOTER / REAR CORRIDOR
            ↓
           ROSE
            ↓
     SAFE-ROOM DOORWAY
            ↓
      CAMERA / SAFE ROOM
```

No crossfire.
No side shooters.
No shooter teleportation.

Later visible impacts were removed when they were not necessary.

Permanent scoped rule:

> In single-take action scenes, define the shooter origin and line-of-fire before specifying impact VFX.

---

### Failure D — final bullets appeared on the wrong side of the door

A render showed the final impacts on the visible face of the door even though Rose and camera were already supposed to be inside and the shooter outside.

### Fix

The final impacts became an **occluded-surface event**:

- shooter stays outside
- door is fully latched
- bullets hit the exterior / corridor-facing surface
- camera cannot see those impact points
- inside the room, communicate the hit only through:
  - muffled metallic sound
  - door vibration
  - subtle handle/panel movement

Permanent scoped rule:

> Never visually render an impact point on a surface that should be hidden from the active camera. Use transmitted sound, vibration or secondary physical response instead.

---

### Failure E — safe-room topology became too complex

Prompts that simultaneously required:

- camera entering first
- Rose following
- door rotation
- visible impacts
- changing framing
- precise line-of-fire

became too difficult for a 10-second one-take render.

### Fix

The last production prompt deliberately simplified the second half:

- no visible impacts after ~5 seconds unless essential
- late rear burst = audio-only
- camera retreats through doorway
- Rose follows
- door closes
- final outside impacts = sound + vibration only

Higher-order rule:

> When Flow repeatedly breaks spatial logic, remove nonessential VFX instead of adding more geometry constraints.

---

## 5) Approved audio direction

- recognizable industrial two-tone emergency siren from frame 0
- siren clearly audible for approximately first 2 seconds
- duck siren under dialogue
- gunfire placed primarily in dialogue gaps
- concrete impacts = dust/chips, no bright spark
- metal impacts = tiny localized sparks only when visible
- final exterior closed-door hits = muffled sound only from inside
- no music required
- no trailer booms
- dialogue remains foregrounded

---

## 6) Cover

The Reel is standalone.

The user explicitly rejected episode numbering.

### Final cover headline

```text
پرامپت‌های سِرّی لو رفت!
```

Do NOT use:

- قسمت ۱
- episode numbering
- promises of a next episode

Visual direction:

- Rose
- industrial spy-thriller environment
- red emergency accent
- black / concrete / metal palette
- strong Persian hierarchy
- readable on profile grid
- no generic AI-tech look

---

## 7) Subtitle / dialogue graphics

The first subtitle PNG attempt was rejected because it looked like plain dark caption cards and did not match the Reel.

Rejected direction:

- simple translucent rectangles
- generic white Persian text
- weak relationship to lighting and genre

Approved creative direction for future subtitle assets:

- industrial metal title plates
- black / steel / dark charcoal base
- red emergency-light accents
- localized sparks / wear
- cinematic tactical-thriller look
- high-contrast Persian typography
- still transparent/editable as overlay when produced for final edit

Rule:

> Reel subtitle graphics should inherit the actual video genre, lighting and material language — not use a generic subtitle template.

---

## 8) Instagram → Telegram funnel

The initial DM-only prompt delivery evolved into a higher-value funnel.

### Final funnel

```text
REEL
↓
comment keyword: «پرامپت»
↓
NovinHub automatic DM
↓
direct link to the exact Telegram post
↓
downloadable PDF guide
```

No follow requirement.
No unnecessary steps.
Use a direct Telegram post link rather than sending the user to the channel homepage.

### DM direction

Keep the DM short.

The value proposition is:

- 7 professional prompts
- real examples
- ready-to-copy text
- free PDF
- available in Telegram

---

## 9) Telegram PDF asset

Final PDF:

`ASDEV_7_Secret_Prompts_Professional_Guide_FA.pdf`

### Final structure

- 19 pages
- Persian-first
- true RTL / right-aligned layout
- mobile-readable typography
- 7 professional prompt systems
- explanation of when to use each prompt
- ready-to-copy prompt block
- real example
- customization guidance
- common mistake / usage note
- bonus instruction set
- final cheat sheet

### Content categories

1. prompt builder / request optimizer
2. research and verification
3. critique and rewriting
4. learning / personal tutor
5. content production
6. decision support
7. action-plan builder

The PDF replaced the earlier version because the first file had weaker RTL, dense spacing and insufficiently explanatory copy.

---

## 10) Telegram promotional image

A rectangular Telegram post image was created in the same visual family:

- Rose
- dark industrial / secret-file environment
- red + black palette
- PDF book mockup
- strong headline around 7 secret professional prompts
- free educational PDF framing
- ASDEV branding

Artifact direction/name used during production:

`asdev_secret_prompt_guide.png`

---

## 11) Distribution copy decisions

### Instagram comment keyword

`پرامپت`

### Funnel promise

Do not position the reward as only one prompt.

Position it as:

- 7 professional prompts
- real examples
- method of use
- downloadable PDF

This gives the Telegram transition a concrete reason.

---

## 12) What is frozen

Do not reopen unless there is a blocking publishing issue:

- `P4.mp4`
- exact Persian dialogue
- Rose identity / hair
- CTA keyword `پرامپت`
- standalone Reel framing
- no episode numbering
- Reel → NovinHub → Telegram PDF funnel

---

## 13) What remains after publication

After the Reel is published, capture:

- views
- average watch time
- non-follower percentage
- follows
- comments
- shares
- saves
- profile visits
- Telegram click-through if available
- PDF post views/download proxy if available

Then compare against current ASDEV internal targets and decide whether the **secret-prompt spy-thriller format** deserves reuse.

---

## Permanent learnings from this cycle

1. Freeze accepted Persian dialogue before visual-only iteration.
2. Explicit action blocking beats generic "high energy" instructions.
3. Shooter topology must be defined before bullet-impact choreography.
4. Hidden-side impacts should be communicated through sound/vibration, not impossible visible VFX.
5. Remove nonessential visible impacts when Flow cannot preserve spatial logic.
6. A successful Reel-to-Telegram funnel should provide a real downloadable asset, not merely duplicate the DM.
7. Subtitle graphics must match the Reel's actual genre and lighting.
8. Do not invent episode numbering for standalone content.

