# Flow Reels — Approved Prompt Library

این فایل فقط promptها و patternهایی را نگه می‌دارد که در گفتگو **تأیید شده‌اند یا خروجی قابل‌قبول داده‌اند**. Promptهای صرفاً پیشنهادی یا تست‌نشده نباید با برچسب APPROVED وارد این فایل شوند.

## Status vocabulary

- `APPROVED-RENDER` — خروجی ساخته شد و کاربر آن مرحله را قبول کرد.
- `APPROVED-PATTERN` — ساختار prompt در خروجی موفق اثبات شده است.
- `WORKFLOW-APPROVED` — روش اجرایی توسط کاربر استفاده/تأیید شده، ولی به یک render خاص محدود نیست.
- `SUPERSEDED` — قبلاً استفاده شده اما نسخه بهتر جایگزین شده است.
- `REJECTED` — failure pattern؛ برای جلوگیری از تکرار نگه داشته می‌شود.

---

# P-001 — Timed Speech + Real Silence Contract

**Status:** `APPROVED-PATTERN`

این pattern از Reel موفق Gemini Live استخراج شده و باید default prompt architecture برای talking Reelهای Flow باشد.

```text
The most important requirement is:

DO NOT SPEAK CONTINUOUSLY.

Rose must speak in SHORT SEPARATE PHRASES with REAL SILENCE between them.

If a phrase finishes early, Rose MUST WAIT until the scheduled next speech block.

Do not fill silence with speech.

The following timing has priority over everything else.
Never begin a speech block early.

During SILENCE:
NO speech.
NO whisper.
NO filler sound.
NO mouthing the next sentence.

Natural human performance is more important than maximizing speech.
```

### چرا موفق است

- timing را از مدل پس می‌گیرد و explicit می‌کند؛
- silence را به acting space تبدیل می‌کند؛
- از machine-gun delivery جلوگیری می‌کند؛
- اجازه نمی‌دهد model جمله بعدی را زود شروع کند.

---

# P-002 — Gemini Live C01 / Suspense Hook

**Status:** `APPROVED-RENDER`

**Duration:** 8s

خروجی Clip 1 مورد قبول بود و به‌عنوان baseline موفق برای performance + silence ثبت می‌شود.

```text
DURATION: EXACTLY 8 SECONDS
FORMAT: Vertical 9:16
ROLE: Clip 1 of a two-clip Instagram Reel

Create a realistic organic Instagram creator video featuring Rose.

THIS CLIP IS ABOUT PERFORMANCE, SUSPENSE AND NATURAL PERSIAN SPEECH.

The most important requirement is:

DO NOT SPEAK CONTINUOUSLY.

Rose must speak in SHORT SEPARATE PHRASES with REAL SILENCE between them.

If a phrase finishes early, Rose MUST WAIT until the scheduled next speech block.

Do not fill silence with speech.

==================================================
ROSE — ABSOLUTE IDENTITY LOCK
==================================================

Rose is a Persian woman approximately 25 years old.

Keep permanently consistent:

- youthful oval face
- warm light-to-medium skin
- dark brown almond-shaped eyes
- full dark eyebrows
- slim nose
- subtle nose piercing
- round thin black eyeglasses
- chin-length bob haircut
- very dark roots
- vivid hot-magenta front and side hair
- sapphire / electric-blue underneath

No identity drift.

==================================================
WARDROBE — MODERN SKEPTICAL INVESTIGATOR
==================================================

Rose wears:

- fitted dark-charcoal top
- cropped stone/beige trench-inspired jacket, open
- high-waisted dark trousers
- slim dark belt
- minimal silver jewelry
- modern black ankle boots

She must look like a stylish modern creator with subtle investigator energy.

NOT cosplay.

NO:
- police badge
- magnifying glass
- detective hat
- costume props

==================================================
ENVIRONMENT
==================================================

Modern creator apartment.

Mood:
subtle mystery, clean and realistic.

Use:

- warm-neutral background
- controlled soft face lighting
- subtle practical lamp
- shallow depth of field
- clean modern environment

No readable text.
No logos.
No fake interfaces.
No extra people.

==================================================
CAMERA
==================================================

Vertical 9:16.

Stable medium framing.

Rose approximately mid-torso upward.

Camera remains essentially locked.

NO:
- orbit
- dramatic zoom
- whip pan
- camera shake
- shot changes

==================================================
ACTING DIRECTION
==================================================

Rose acts like a smart suspicious investigator who has discovered something unusual.

She is:

- skeptical
- curious
- intelligent
- slightly teasing
- alert
- expressive but restrained

Facial acting is especially important DURING SILENCE.

Use:

- suspicious eye contact
- subtle squint
- eyebrow movement
- tiny head tilt
- natural blinking
- natural breathing
- controlled micro-smiles

Do NOT overact.

==================================================
ABSOLUTE AUDIO TIMELINE
==================================================

The following timing has priority over everything else.

Never begin a speech block early.

During SILENCE:
NO speech.
NO whisper.
NO filler sound.
NO mouthing the next sentence.

--------------------------------------------------
0.00–1.15 SEC — SPEECH BLOCK 1
--------------------------------------------------

Rose is looking suspiciously at her smartphone.

She quickly looks directly at the viewer.

Say:

«گوشیتو می‌گرده؟»

DELIVERY:

Suspicious.
Provocative.
Curious.

It must sound like a genuine question.

Do not shout.

Finish the phrase naturally.

Then STOP.

--------------------------------------------------
1.15–1.85 SEC — SILENCE
--------------------------------------------------

FULL SILENCE for approximately 0.70 seconds.

Rose does NOT speak.

She:

- maintains direct eye contact
- slightly narrows her eyes
- makes a tiny head tilt

This silence must be visually noticeable.

--------------------------------------------------
1.85–3.15 SEC — SPEECH BLOCK 2
--------------------------------------------------

Say:

«صفحه گوشیتو می‌بینه...»

Delivery:

Slow.
Suspicious.
Matter-of-fact.

Do NOT immediately explain further.

Finish and STOP.

--------------------------------------------------
3.15–3.75 SEC — SILENCE
--------------------------------------------------

FULL SILENCE for approximately 0.60 seconds.

Rose briefly glances toward her phone.

Then looks back at the viewer.

NO SPEECH.

--------------------------------------------------
3.75–5.75 SEC — SPEECH BLOCK 3
--------------------------------------------------

Say:

«حتی می‌فهمه چه برنامه‌ای باز کردی.»

Delivery:

Clear.
Natural.
Slightly surprised.

This should feel like Rose revealing the strange part she discovered.

Do NOT rush the final words.

Then STOP.

--------------------------------------------------
5.75–6.35 SEC — SILENCE
--------------------------------------------------

FULL SILENCE for approximately 0.60 seconds.

Rose holds eye contact.

Tiny skeptical half-smile.

NO SPEECH.

--------------------------------------------------
6.35–7.30 SEC — SPEECH BLOCK 4
--------------------------------------------------

Say:

«عجیبه... نه؟»

IMPORTANT:

Say:

«عجیبه...»

brief internal pause

then:

«نه؟»

This must sound playful and skeptical.

Not like a narrator.

--------------------------------------------------
7.30–8.00 SEC — ENDING SILENCE
--------------------------------------------------

NO MORE SPEECH.

Rose holds:

- suspicious half-smile
- direct eye contact
- smartphone in stable position

IMPORTANT:

The final body pose, phone position, facial direction, lighting and framing must remain stable.

The final frame will be used as the visual reference for Clip 2.

==================================================
EXACT SPOKEN PERSIAN
==================================================

The complete dialogue is:

«گوشیتو می‌گرده؟ صفحه گوشیتو می‌بینه. حتی می‌فهمه چه برنامه‌ای باز کردی. عجیبه... نه؟»

BUT:

DO NOT read this continuously.

The timed blocks and silent sections above are mandatory.

==================================================
VOICE
==================================================

Natural young Iranian Persian female voice.

NOT formal Persian.
NOT advertisement speech.
NOT a news presenter.

The performance must have:

- changing pitch
- changing speed
- breathing
- emotion
- hesitation
- real silence
- conversational rhythm

ABSOLUTELY AVOID:

- machine-gun speech
- robotic cadence
- monotone delivery
- constant speaking speed
- rushing
- starting the next phrase during silence

Natural human performance is more important than maximizing speech.

==================================================
NO TEXT
==================================================

Do NOT generate:

- subtitles
- captions
- Persian text
- English text
- logos
- interfaces
- readable phone content
```

---

# P-003 — Rose Identity / Hair Lock

**Status:** `APPROVED-PATTERN`

برای promptهای مستقل که reference image ندارند، این lock از drift رنگ مو جلوگیری می‌کند.

```text
ROSE — ABSOLUTE IDENTITY LOCK

Rose is a Persian woman approximately 25 years old.

Keep her identity completely stable and consistent throughout the video.

Preserve permanently:

- youthful oval face
- warm light-to-medium skin
- dark brown almond-shaped eyes
- full dark eyebrows
- slim nose
- subtle nose piercing
- round thin black eyeglasses
- chin-length bob haircut
- VERY DARK BROWN / NEAR-BLACK ROOTS
- vivid HOT-MAGENTA hair on the front and outer side sections
- deep SAPPHIRE / ELECTRIC-BLUE hair underneath and through the lower inner sections

CRITICAL HAIR IDENTITY:

Rose's hair is NOT fully pink.
Rose's hair is NOT purple.
Rose's hair is NOT fully blue.

The required permanent color pattern is:

VERY DARK ROOTS
+
HOT-MAGENTA FRONT / OUTER SECTIONS
+
SAPPHIRE-BLUE UNDERLAYER.

The blue underlayer must remain visibly recognizable.

Hair length must remain CHIN-LENGTH.

ABSOLUTELY NO:
- identity drift
- different woman
- face redesign
- ponytail
- long hair
- removing glasses
- fully magenta hair
- fully purple hair
- fully blue hair
```

---

# P-004 — One-Minute Tutorial Teaser

**Status:** `APPROVED-RENDER`

**Duration:** 10s

هدف: Reel آموزش را لو نمی‌دهد؛ فقط مسئله → promise → Telegram CTA.

Exact spoken Persian نسخه‌ای که برای render نهایی استفاده شد:

```text
«بَرایِ پیجَت ریلز می‌خوای بِسازی؟ وَلی گوگِل فِلو فَقَط دَه ثانیه ویدیو می‌ده؟ بیا بِهت یاد بِدَم چِطور یِک‌دَقیقه‌ای بِسازی. آموزشِ کامل، تو کانالِ تِلِگرام.»
```

### Timing contract

```text
0.00–1.75 — «بَرایِ پیجَت ریلز می‌خوای بِسازی؟»
1.75–2.10 — full silence
2.10–4.45 — «وَلی گوگِل فِلو فَقَط دَه ثانیه ویدیو می‌ده؟»
4.45–4.80 — full silence
4.80–6.95 — «بیا بِهت یاد بِدَم چِطور یِک‌دَقیقه‌ای بِسازی.»
6.95–7.30 — full silence
7.30–9.25 — «آموزشِ کامل، تو کانالِ تِلِگرام.»
9.25–10.00 — no speech; hold downward pointing pose
```

### Telegram gesture contract

```text
As she begins saying:
«تو کانالِ تِلِگرام»

she raises ONE hand naturally,
extends ONE index finger,
and points CLEARLY DOWNWARD toward the LOWER-CENTER of the frame.

The lower-center region must remain EMPTY.

Hold the downward pointing pose through the final frame.

Do NOT generate:
- Telegram username
- Telegram logo
- arrows
- subtitles
- captions
```

### Pronunciation lock

```text
«گوگِل»
«فِلو»
«یِک‌دَقیقه‌ای»
«تِلِگرام»
```

---

# P-005 — Chained Clip Continuity Block

**Status:** `WORKFLOW-APPROVED`

برای C02 به بعد در ویدیوهای 20/30/60 ثانیه‌ای:

```text
The PROVIDED IMAGE is the exact final frame
of the previous clip.

Create the NEXT 10-second clip as a seamless
continuation of the SAME recording.

ABSOLUTE CONTINUITY LOCK:

Preserve exactly:
- character identity and face
- hairstyle and exact hair colors
- clothing and accessories
- body proportions
- environment and background
- lighting
- camera height, angle and distance
- framing
- color palette
- starting body orientation

The FIRST FRAME must closely match
the provided reference image.

DO NOT:
- redesign the character
- change wardrobe
- change hairstyle or hair colors
- change the room
- change lighting
- reset the pose
- change camera position
- create a new shot unless explicitly requested

Begin from the reference pose,
then continue the new action naturally.

DIALOGUE / ACTION FOR THIS CLIP:
[متن و اکشن این ۱۰ ثانیه]

ENDING:
During the final 0.7 seconds:
- stabilize the pose
- reduce large movement
- keep face and hands readable

The final frame will be used
as the reference for the next clip.
```

---

# Superseded / Rejected Patterns

## R-001 — Dense 10-second tutorial dialogue

**Status:** `REJECTED`

علامت failure:

- چند concept + method + CTA در یک 10s clip
- نتیجه: speech سریع، robotic و کم‌اثر

Rule:

> Reel teaser آموزش را توضیح نمی‌دهد؛ آموزش به Caption / pinned comment / Telegram منتقل می‌شود.

## R-002 — Foreign product name + Persian suffix when pronunciation breaks

**Status:** `SUPERSEDED`

نمونهٔ مشکل‌دار:

`لایوئه / لایوه`

راه‌حل:

اسم مستقل و ساده:

`جِمِنای لایو`

یا sentence structure بدون suffix.

## R-003 — Reference-image language when no image should be supplied

**Status:** `REJECTED`

عبارت‌هایی مثل:

`The provided reference image...`

وقتی user نمی‌خواهد عکس به Flow بدهد، باعث می‌شوند Gemini درخواست image کند.

Rule:

> No-reference prompt باید کاملاً self-contained باشد و هیچ اشاره‌ای به provided image / reference image نداشته باشد.

## R-004 — Technical model name in consumer hook

**Status:** `REJECTED for general-audience hook`

اگر نام فنی برای فهم outcome لازم نیست، در speech حذف شود. نام دقیق مدل می‌تواند در caption / pinned comment / tutorial بیاید.

---

# Promotion Rule

Prompt جدید فقط وقتی به این فایل اضافه شود که یکی از این evidenceها وجود داشته باشد:

1. user صریحاً خروجی را approve کند؛
2. output ساخته شود و workflow بدون درخواست regenerate وارد مرحله Cover/Publish شود؛
3. pattern در حداقل دو task مستقل موفق باشد.

Prompt تست‌نشده را در این فایل APPROVED نکن.
