# Flow Reels — Approved AI-Tool Prompt Baselines — 2026-09-03

این فایل prompt baselineهای تأییدشدهٔ چرخه Copilot → Z.ai → Duck.ai را نگه می‌دارد.

Status vocabulary:

- `APPROVED-RENDER` — خروجی render شده و user آن را پذیرفته است.
- `APPROVED-PATTERN` — معماری prompt در render موفق اثبات شده است.
- `SUPERSEDED` — نسخه قبلی که با evidence بهتر جایگزین شده است.

---

# P-006 — 10s Persian Speech Architecture from Successful Skincare Prompt

**Status:** `APPROVED-PATTERN`

این pattern از prompt موفقی که user ارائه کرد استخراج شده است و برای talking Reelهای فارسی با reference image baseline خوبی است.

```text
Create a 10-second photorealistic vertical Instagram Reel.

VIDEO FORMAT:
- Duration: exactly 10 seconds
- Aspect ratio: 9:16 vertical
- Photorealistic
- Realistic human motion
- Realistic Persian lip synchronization
- One continuous primary shot
- No rapid cuts

REFERENCE CHARACTER:
Use the provided reference image as the main visual reference.
Preserve the same overall appearance and identity throughout the entire video.
Do not change face, hairstyle, clothing or facial features between frames.

SCENE:
[Simple realistic environment matching the topic]

CAMERA:
Start with a medium close-up.
Camera at eye level.
50mm portrait lens aesthetic.
Very subtle, slow cinematic push-in.
The camera remains smooth and stable.
Do not cut away while the character is speaking.

PERFORMANCE:
0.0–0.8 seconds:
Look naturally into the camera.
Small natural breathing and facial movement.

0.8–3.2 seconds:
Speak the first sentence directly to the viewer.

3.2–3.5 seconds:
Very short natural pause.

3.5–7.7 seconds:
Speak the second sentence.
One subtle hand gesture maximum.

7.7–8.0 seconds:
Very short natural pause.

8.0–9.6 seconds:
Speak the final sentence directly to camera.

9.6–10.0 seconds:
Finish speaking and hold a natural final expression.

IMPORTANT SPEECH INSTRUCTIONS:
The visible character speaks the dialogue.
This is NOT a voice-over.

Language:
ONLY Persian / Farsi.

Accent:
Natural contemporary Iranian Persian.
Natural Tehran-style pronunciation.

Speaking speed:
moderate and conversational.
Do not speak too quickly.
Use natural short pauses between sentences.

CRITICAL:
Speak the Persian dialogue EXACTLY as written.

DO NOT:
- paraphrase
- translate
- rewrite
- add words
- remove words
- repeat words
- stutter
- stretch syllables
- elongate vowels
- elongate consonants
- repeat final consonants

EXACT SPOKEN DIALOGUE:
[INSERT THE SHORTEST APPROVED DIALOGUE]

PRONUNCIATION REQUIREMENTS:
Only add locks for words that have demonstrated pronunciation risk.
Every Persian word must be spoken once and naturally.
Do not exaggerate any word.
Do not prolong final sounds.
Do not produce robotic rhythm.
Do not pause inside individual phrases.

FACIAL AND BODY PERFORMANCE:
Maintain direct natural eye contact.
Natural blinking.
Subtle facial expressions.
Very small natural head movement.
One or two restrained hand gestures maximum.
No exaggerated influencer gestures.

AUDIO:
Clean studio-quality dialogue.
Persian speech is dominant.
Very subtle room ambience only.

STRICT NEGATIVE CONSTRAINTS:
No subtitles.
No captions.
No on-screen Persian text.
No English text.
No logo.
No username.
No watermark generated inside the scene.
No extra dialogue.
No background people.
No fast cuts.
No changing identity.
No lip-sync mismatch.
No repeated words.
No elongated Persian words.
```

## Why this pattern is approved

- section hierarchy ساده است؛
- exact dialogue یک authoritative block دارد؛
- pronunciation lock targeted است؛
- negative rules محدود و مرتبط‌اند؛
- model را با instructionهای متناقض over-control نمی‌کند.

---

# P-007 — Z.ai No-Reference 10s Creator Pattern

**Status:** `APPROVED-RENDER` + `APPROVED-PATTERN`

**Mode:** no reference image

**Core dialogue:**

```text
«پول نده، سایتتو رایگان بساز!»

[REAL SILENCE]

«فقط بگو چه سایتی میخوای، خودش برات می‌سازه.»

[REAL SILENCE]

«بدون کدنویسی.»

[REAL SILENCE]

«اگه میخوایش؟ سایت و کامنت کن.»
```

**Canonical timing:**

```text
0.00–1.55 — hook
1.55–2.30 — real silence
2.30–4.55 — main benefit
4.55–5.15 — real silence
5.15–6.20 — short benefit
6.20–6.80 — real silence
6.80–8.55 — CTA
8.55–10.00 — silent end hold
```

**Reusable prompt:**

```text
=====================
DURATION: EXACTLY 10 SECONDS
FORMAT: Vertical 9:16
ROLE: Complete standalone Instagram Reel
LANGUAGE: Natural conversational Iranian Persian

Create a realistic, organic, high-retention Instagram creator video featuring an ORIGINAL fictional young woman.

NO reference image will be provided.

The entire character appearance, environment, performance, voice rhythm, and dialogue must be created only from the written description below.

==================================================
CORE VIDEO CONCEPT
==================================================

The video promotes an unnamed AI website-building tool.

The viewer should understand that:
- they can build a website for free
- they do not need coding knowledge
- they only need to describe the website they want
- the AI handles the creation

The AI tool name must NOT be revealed anywhere inside the video.

The video structure must be:
AGGRESSIVE HOOK
→ REAL SILENT PAUSE
→ SIMPLE BENEFIT
→ REAL SILENT PAUSE
→ SHORT SECOND BENEFIT
→ REAL SILENT PAUSE
→ COMMENT CTA
→ SILENT END HOLD

==================================================
HIGHEST PRIORITY — NATURAL SPEECH
==================================================

THE VIDEO MUST NOT SOUND ROBOTIC.
DO NOT read all sentences as one paragraph.
DO NOT use continuous speech.
DO NOT use machine-gun delivery.
DO NOT rush to fill the full 10 seconds.

REAL SILENCE between sentences is required.

During every silent pause:
- completely stop speaking
- close the mouth
- stop all lip movement associated with speech
- naturally breathe
- maintain eye contact
- natural blinking is allowed

If there is unused time:
KEEP SILENCE.

==================================================
CHARACTER — FIXED VISUAL IDENTITY
==================================================

Create an ORIGINAL fictional woman approximately 27–33 years old.

She is a realistic intelligent brunette creative professional.

Core identity:
- soft oval / slightly elongated face
- fair to light neutral-warm skin
- hazel-brown / warm brown eyes
- naturally full dark-brown eyebrows
- black full-rim rounded-square eyeglasses
- long dark brunette hair
- slightly off-center side part
- natural loose waves
- black long-sleeve top
- minimal accessories
- warm realistic creative workspace

She must NOT look like a fashion model or stereotypical influencer.

==================================================
CAMERA
==================================================

ONE SINGLE CONTINUOUS SHOT.
Vertical 9:16.
Stable medium close-up.
Approximately chest-up.
Eye level.
Natural 40–55mm equivalent perspective.
Almost completely stationary.

NO dramatic zoom, orbit, whip pan, tracking movement, camera shake, cuts or B-roll.

==================================================
ABSOLUTE AUDIO + SILENCE TIMELINE
==================================================

0.00–1.55 SEC
Say EXACTLY:
«پول نده، سایتتو رایگان بساز!»

This sentence has the highest energy.
Approximately 15–20% louder than the other sentences.
Do NOT shout.

1.55–2.30 SEC
ABSOLUTELY NO SPEECH.
Mouth closed.
Natural breathing.

2.30–4.55 SEC
Say EXACTLY:
«فقط بگو چه سایتی میخوای، خودش برات می‌سازه.»

Natural conversational volume.
Do NOT rush.
Do NOT replace the verb form.

4.55–5.15 SEC
NO SPEECH.

5.15–6.20 SEC
Say EXACTLY:
«بدون کدنویسی.»

Say ONLY this short sentence.
Do NOT expand it.

6.20–6.80 SEC
NO SPEECH.

6.80–8.55 SEC
Say EXACTLY:
«اگه میخوایش؟ سایت و کامنت کن.»

Friendly, direct, slightly playful.

8.55–10.00 SEC
NO MORE SPEECH.
Hold direct eye contact and subtle confident smile.

==================================================
EXACT SPOKEN AUDIO
==================================================

Speak EXACTLY these four blocks ONCE:

«پول نده، سایتتو رایگان بساز!»

[REAL SILENCE]

«فقط بگو چه سایتی میخوای، خودش برات می‌سازه.»

[REAL SILENCE]

«بدون کدنویسی.»

[REAL SILENCE]

«اگه میخوایش؟ سایت و کامنت کن.»

Nothing else.

==================================================
CRITICAL PRONUNCIATION
==================================================

The exact word is:
«میخوایش»

It must sound like ONE smooth natural casual Iranian Persian word.
Do not add an extra syllable or extra «ی» sound.
Do not stretch the vowel.
Do not separate the ending.

Use EXACTLY:
«خودش برات می‌سازه.»

Do NOT substitute:
«می‌سازتش»

==================================================
NO PRODUCT REVEAL / NO GENERATED TEXT
==================================================

Never mention the product name.
Do not generate subtitles, captions, readable Persian/English text, logos, usernames, UI or watermarks.

==================================================
FINAL SUCCESS TEST
==================================================

Success requires:
- realistic brunette creative professional
- black rounded-square glasses
- black long-sleeve top
- warm blurred workspace
- energetic but natural hook
- real silence after each block
- clear «خودش برات می‌سازه»
- standalone «بدون کدنویسی.»
- correct «میخوایش»
- no product reveal
- no generated text
- final silent hold
=====================
```

---

# P-008 — Duck.ai Reference-Image 10s Talking Creator

**Status:** `APPROVED-RENDER`

**Reference:** user's first portrait — direct eye contact, black suit/shirt/tie, executive chair, office shelves.

**Product reveal:** hidden in spoken video; reveal on cover/caption/comment replies.

## Final accepted spoken dialogue

```text
«پول اشتراک نده. حتی ثبت نام هم نکن!»

«چندتا هوش مصنوعی معروف رو رایگان یه جا داری.»

«عکس هم می‌سازه.»

«اگه میخوایش همه رو کامنت کن.»
```

## Critical supersessions

```text
SUPERSEDED:
«پول اشتراک نده، حتی ثبت‌نامم نکن!»

CURRENT:
«پول اشتراک نده. حتی ثبت نام هم نکن!»
```

```text
SUPERSEDED:
«اگه میخوایش؟ همه رو کامنت کن.»

CURRENT:
«اگه میخوایش همه رو کامنت کن.»
```

Reason: question-mark/internal pause + keyword emphasis caused duplicate/restart around «همه» in one render.

## Canonical production prompt

```text
Create a 10-second photorealistic vertical Instagram Reel.

VIDEO FORMAT:
- Duration: exactly 10 seconds
- Aspect ratio: 9:16 vertical
- Photorealistic
- Realistic human motion
- Realistic Persian lip synchronization
- One continuous shot
- No cuts
- No B-roll

REFERENCE CHARACTER:
Use the provided reference image as the main visual reference for the man.
Preserve the SAME identity throughout the entire video.

Keep his appearance closely matched to the reference:
- adult Iranian / Persian man
- short dark hair
- dark brown eyes
- strong dark eyebrows
- short naturally trimmed beard
- small distinctive goatee area under the lower lip
- medium-light olive skin tone
- masculine facial structure
- serious and confident appearance

WARDROBE:
- black suit
- black shirt
- dark tie
- clean monochrome professional styling

SCENE:
A realistic modern executive office similar to the reference image.
Background:
- black executive chair
- softly blurred office shelving
- folders or binders
- subtle professional office objects
- clean modern interior

CAMERA:
One continuous medium close-up.
Approximately chest-up.
Camera at eye level.
50mm portrait-lens aesthetic.
Stable camera.
The camera should remain almost stationary.
No dramatic push-in.
No zoom.
No camera shake.
No angle changes.

==================================================
PERFORMANCE
==================================================

The man speaks directly to one viewer.
He should feel like a real Iranian creator sharing a useful discovery.

IMPORTANT:
HIGH ENERGY DOES NOT MEAN FAST SPEECH.

The hook should feel powerful because of:
- stronger eye contact
- confident facial expression
- slightly stronger voice
- controlled emphasis

NOT because of faster speaking.

Do not rush the beginning.

==================================================
TIMING
==================================================

0.0–1.0 SECONDS:
ABSOLUTELY NO SPEECH.
The man looks directly into the camera.
Mouth naturally closed.
Natural breathing.

1.0–3.15 SECONDS:
Speak the FIRST dialogue line.
Controlled confident pace.
The hook is slightly stronger and louder than the following dialogue, but NOT faster.

3.15–3.50 SECONDS:
SHORT NATURAL SILENCE.

3.50–5.85 SECONDS:
Speak the SECOND dialogue line.
Normal conversational volume.
Relaxed and clear.
Every word spoken once.

5.85–6.15 SECONDS:
SHORT NATURAL SILENCE.

6.15–7.05 SECONDS:
Speak the THIRD dialogue line.
Short, simple, natural.

7.05–7.35 SECONDS:
SHORT NATURAL SILENCE.

7.35–8.80 SECONDS:
Speak the FINAL dialogue line.
Friendly and conversational.
Use ONE continuous natural phrase.

IMPORTANT:
Do NOT create a pause inside this sentence.
Do NOT isolate the comment keyword.
Do NOT emphasize the comment keyword.
Do NOT restart the last part of the sentence.
Do NOT repeat any word.

8.80–10.00 SECONDS:
NO MORE SPEECH.
Hold direct eye contact, subtle confident half-smile and natural breathing.

==================================================
EXACT SPOKEN DIALOGUE
==================================================

The visible man himself speaks.
This is NOT voice-over.
Language: ONLY Persian / Farsi.
Accent: Natural contemporary Iranian Persian.
Natural Tehran-style conversational pronunciation.

Speak EXACTLY:

«پول اشتراک نده. حتی ثبت نام هم نکن!

چندتا هوش مصنوعی معروف رو رایگان یه جا داری.

عکس هم می‌سازه.

اگه میخوایش همه رو کامنت کن.»

Nothing else.

==================================================
CRITICAL SPEECH REQUIREMENTS
==================================================

Every Persian word must be spoken exactly ONCE.

DO NOT:
- paraphrase
- translate
- rewrite
- add words
- remove words
- repeat words
- repeat syllables
- restart a sentence
- stutter
- stretch vowels
- stretch consonants
- repeat final consonants
- speak too quickly
- use machine-gun delivery

==================================================
FIRST LINE — CRITICAL
==================================================

The first line is:
«پول اشتراک نده. حتی ثبت نام هم نکن!»

Do NOT rush this sentence.
The first word begins only AFTER the initial silent hold.

Pronounce:
«پول اشتراک نده»
clearly and at a controlled pace.

Then make a very small natural sentence break.

Then pronounce:
«حتی ثبت نام هم نکن»
clearly.

Do not merge:
«ثبت نام هم»
into an unclear word.

Do not say:
«ثبت نامم»

==================================================
FINAL LINE — HIGHEST PRIORITY
==================================================

Say exactly:
«اگه میخوایش همه رو کامنت کن.»

as ONE smooth continuous conversational phrase.

There is NO intentional pause inside this sentence.
Do not stop after «میخوایش».
Continue naturally.

The word immediately following «میخوایش» must be spoken only ONCE.
Do not:
- repeat it
- attack it twice
- restart it
- cut it in half
- stretch it
- isolate it
- strongly emphasize it

==================================================
PRONUNCIATION — «میخوایش»
==================================================

Pronounce «میخوایش» as ONE smooth casual Iranian Persian word.
Do not over-articulate it.
Do not insert an additional syllable.
Do not add an extra «ی» sound.
Do not stretch the ending.

==================================================
PRODUCT PRIVACY / NO GENERATED TEXT
==================================================

Do not reveal the service name.
Do not speak or display Duck.ai / DuckDuckGo / logo / URL / recognizable UI.

No subtitles.
No captions.
No Persian text.
No English text.
No logo.
No username.
No watermark.
No UI.

==================================================
FINAL SUCCESS REQUIREMENTS
==================================================

Success if:
1. same identity as reference image
2. black professional appearance remains consistent
3. natural Iranian Persian voice
4. hook confident but not rushed
5. each line spoken once
6. no repetition / stutter / restart
7. CTA is one continuous fluent phrase
8. «میخوایش» natural
9. no product reveal
10. no generated text
11. final section silent
```

## Render QA note

در render پذیرفته‌شده، شروع دقیقاً یک ثانیه silence کامل نبود، ولی output برای مخاطب طبیعی و قابل‌انتشار بود. Rule عملی:

> اگر deviation زمانی جزئی است اما artifact شنیداری/بصری واضح وجود ندارد، فقط برای انطباق میلی‌ثانیه‌ای credit دوباره خرج نکن.

---

# P-009 — CTA Anti-Restart Micro-Pattern

**Status:** `APPROVED-PATTERN`

برای CTAهایی که keyword در آن‌ها repeat / cut / restart می‌شود:

```text
Say the final CTA as ONE smooth continuous conversational phrase.

Do NOT create an internal pause before the keyword.
Do NOT isolate the keyword.
Do NOT strongly emphasize the keyword.
Do NOT restart the keyword.
Do NOT repeat the keyword.
Do NOT attack the first syllable twice.

Every word must be spoken exactly once.
```

### Persian copy rule

ترجیحاً punctuation اضافه قبل از keyword حذف شود.

مثال:

```text
BAD / RISKY:
«اگه میخوایش؟ همه رو کامنت کن.»

BETTER:
«اگه میخوایش همه رو کامنت کن.»
```

---

# P-010 — Energy ≠ Speed Micro-Pattern

**Status:** `APPROVED-PATTERN`

```text
HIGH ENERGY DOES NOT MEAN FAST SPEECH.

The hook should feel powerful because of:
- stronger eye contact
- confident facial expression
- slightly stronger voice
- controlled emphasis

NOT because of faster speaking.

The hook must remain at normal conversational speaking speed.
```

---

# Usage Rule

برای Reel بعدی:

1. از P-006 به‌عنوان base architecture شروع کن.
2. اگر no-reference character است، P-007 را adapt کن.
3. اگر user reference image دارد، P-008 را adapt کن.
4. فقط observed failureهای واقعی را با P-009/P-010 اضافه کن.
5. constraint جدید بدون evidence اضافه نکن.
6. exact dialogue را قبل از prompt قفل کن.
7. اگر credit محدود است، یک prompt production-ready بده، نه چند render variant.
