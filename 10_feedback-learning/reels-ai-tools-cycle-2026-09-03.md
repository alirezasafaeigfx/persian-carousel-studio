# Reels AI Tools Cycle — Copilot → Z.ai → Duck.ai — 2026-09-03

این سند حافظهٔ اجرایی چرخهٔ اخیر Reelهای ابزارهای هوش مصنوعی ASDEV است. هدف آن کاهش آزمون‌وخطا، جلوگیری از فراموشی تصمیم‌های موفق، و شروع Reelهای بعدی از baselineهای تأییدشده است.

> Scope: Microsoft Copilot، Z.ai / Z Chat، Duck.ai، Google Flow / Gemini video generation، Persian speech، reference-image prompting، cover design، caption، comment replies.

---

# 1. فرمول محتوایی قفل‌شده

فرمولی که در این چرخه بهترین نتیجه را داد:

`هوک تهاجمی → مکث واقعی → مزیت خیلی ساده → مکث → مزیت دوم کوتاه → مکث → CTA کامنت → پایان ساکت`

قواعد:

- اسم ابزار داخل spoken Reel گفته نشود اگر curiosity/reveal برای cover/caption مهم است.
- محصول در cover / caption / comment reply reveal شود.
- یک Reel فقط یک CTA اصلی داشته باشد.
- اگر جمله فقط با سریع‌خوانی داخل 10 ثانیه جا می‌شود، متن باید کوتاه شود، نه سرعت زیاد.
- benefit باید برای مخاطب عمومی قابل‌فهم باشد؛ نام فنی مدل هوش مصنوعی hook نیست مگر خود نام اهمیت داستانی داشته باشد.

---

# 2. Copilot — baseline تأییدشده

## Hook / dialogue قفل‌شده در چرخه

`دیگه پول نده، رایگان شد!`

بعد از مکث:

`هم عکس می‌سازه، هم عکساتو ادیت می‌کنه.`

بعد:

`چت هوشمند داره و فارسی هم عالی حرف می‌زنه.`

CTA:

`می‌خوایش؟ کامنت کن «رایگان».`

## Learning

- اسم Copilot داخل ویدیو reveal نشد؛ در cover/caption/comment reply معرفی شد.
- hook باید louder / more excited باشد، ولی pause واقعی بعدش ضروری است.
- silent pause باید با `mouth closed` و `no filler` تعریف شود.
- کاربر خروجی نهایی را عالی ارزیابی کرد و این pattern به baseline Reelهای بعدی تبدیل شد.

---

# 3. Z.ai — baseline تأییدشده

## Hook نهایی

`پول نده، سایتتو رایگان بساز!`

## Dialogue تأییدشده

`پول نده، سایتتو رایگان بساز!`

[REAL SILENCE]

`فقط بگو چه سایتی میخوای، خودش برات می‌سازه.`

[REAL SILENCE]

`بدون کدنویسی.`

[REAL SILENCE]

`اگه میخوایش؟ سایت و کامنت کن.`

## Timing تأییدشده

- 0.00–1.55 hook
- 1.55–2.30 silence ~0.75s
- 2.30–4.55 main benefit
- 4.55–5.15 silence ~0.60s
- 5.15–6.20 short benefit
- 6.20–6.80 silence ~0.60s
- 6.80–8.55 CTA
- 8.55–10.00 silent end hold

## Pronunciation learnings

### «میخوایش»

این token در Flow حساس است.

Canonical spoken token:

`میخوایش`

نباید در همان prompt شکل‌های جایگزین متعدد یا spellingهای رقابتی برای گفتار اصلی ساخته شوند.

### «می‌سازتش»

در render بد تلفظ شد.

راه‌حل تأییدشده:

`خودش برات می‌سازه.`

### «بدون کدنویسی»

نسخه کوتاه standalone بهتر از توضیح طولانی است.

Canonical:

`بدون کدنویسی.`

نه:

`کدنویسی هم لازم نیست.`

## Character / no-reference learning

وقتی reference image به Flow داده نمی‌شود، prompt باید کاملاً self-contained باشد و هیچ عبارت `provided reference image` نداشته باشد.

Character موفق Z.ai:

- زن حدود 27–33
- brunette تیره، side part، loose waves
- black rounded-square glasses
- black long-sleeve top
- warm creative workspace
- realistic / intelligent / professional، نه fashion-model

این description یک no-reference character baseline موفق است.

---

# 4. Duck.ai — cycle کامل و render پذیرفته‌شده

## انتخاب موضوع

Duck.ai به‌جای Gamma انتخاب شد چون hook قوی‌تری برای audience داشت:

- بدون پرداخت اشتراک برای شروع
- بدون ثبت‌نام برای شروع
- چند مدل هوش مصنوعی در یک محیط
- قابلیت ساخت تصویر

ادعای `نامحدود` استفاده نشود مگر جداگانه و در زمان انتشار اثبات شود. نسخه رایگان ممکن است محدودیت مصرف داشته باشد.

## Hook قفل‌شده

نسخه اولیه:

`پول اشتراک نده، حتی ثبت‌نامم نکن!`

### اصلاح تلفظی

`ثبت‌نامم نکن` برای موتور گفتار ریسک بالاتری داشت.

نسخه production-safe و نهایی:

`پول اشتراک نده. حتی ثبت نام هم نکن!`

این rewrite semantic impact را حفظ کرد ولی parsing گفتاری را ساده‌تر کرد.

## Dialogue نهایی render پذیرفته‌شده

`پول اشتراک نده. حتی ثبت نام هم نکن!`

[SHORT NATURAL PAUSE]

`چندتا هوش مصنوعی معروف رو رایگان یه جا داری.`

[SHORT NATURAL PAUSE]

`عکس هم می‌سازه.`

[SHORT NATURAL PAUSE]

`اگه میخوایش همه رو کامنت کن.`

## چرا CTA تغییر کرد؟

نسخه مشکل‌دار:

`اگه میخوایش؟ همه رو کامنت کن.`

در یک render، کلمه «همه» دوبار گفته شد و روی همان کلمه حس cut/restart ایجاد شد.

Corrective action:

- question mark بعد از `میخوایش` حذف شد.
- internal pause حذف شد.
- دستور emphasis روی `همه` حذف شد.
- کل CTA به ONE continuous phrase تبدیل شد.

نسخه canonical:

`اگه میخوایش همه رو کامنت کن.`

### Rule

اگر keyword در CTA repeat/restart می‌شود:

1. punctuation قبل از keyword را حذف کن.
2. keyword را isolate نکن.
3. دستور `emphasize keyword` را حذف کن.
4. sentence را one continuous phrase تعریف کن.
5. صریحاً بگو `Do not restart / repeat / attack the word twice`.

---

# 5. Duck.ai — failure analysis

## Failure A — opening too fast

### Symptom

هوک از frameهای اول خیلی سریع شروع شد؛ مدل `high energy / aggressive hook` را به speed بیشتر ترجمه کرد.

### Root cause

Prompt به‌طور همزمان:

- strong / aggressive / scroll-stopping
- زمان کوتاه برای speech block

داده بود.

### Corrective rule

Canonical instruction:

`HIGH ENERGY DOES NOT MEAN FAST SPEECH.`

و:

`The hook should feel powerful because of stronger eye contact, facial expression and slightly stronger voice — NOT because of faster speaking.`

### Optional safe start

برای Reelهای حساس:

`0.0–1.0s = absolutely no speech, mouth closed, direct eye contact.`

ولی QA واقعی مهم‌تر از انطباق میلی‌ثانیه‌ای است. اگر render از نظر مخاطب طبیعی و بدون artifact است، برای اختلاف کوچک timing نباید credit اضافی سوزانده شود.

---

## Failure B — repeated words / stutter

### Symptom

- تکرار کلمات وسط جمله
- restart syllable
- تکرار «همه»
- حس قطعه‌قطعه شدن audio

### Corrective rules

در prompt speech section:

- `Every Persian word must be spoken exactly ONCE.`
- `Do not repeat words.`
- `Do not restart sentences.`
- `Do not repeat syllables.`
- `Do not stutter.`
- `Do not stretch vowels or consonants.`

اما تجربه این چرخه نشان داد **فقط اضافه کردن negative instruction کافی نیست**؛ syntax خود جمله هم باید ساده شود.

### Higher-order learning

> Simplify the spoken sentence before adding more constraints.

---

# 6. Prompt architecture — چه چیزی واقعاً جواب داد؟

دو prompt موفق قبلی که user ارائه کرد (skincare + Z.ai) نشان دادند architecture ساده و section-based بهتر از over-engineered audio prompt جواب می‌دهد.

Canonical order:

```text
VIDEO FORMAT
REFERENCE CHARACTER / CHARACTER
SCENE
CAMERA
PERFORMANCE + timeline
IMPORTANT SPEECH INSTRUCTIONS
EXACT SPOKEN DIALOGUE
PRONUNCIATION REQUIREMENTS
FACIAL / BODY PERFORMANCE
AUDIO
VISUAL STYLE
STRICT NEGATIVE CONSTRAINTS
FINAL SUCCESS TEST
```

### Strength

- model hierarchy واضح می‌ماند.
- exact dialogue فقط یک‌بار به‌عنوان authoritative block تعریف می‌شود.
- pronunciation lock فقط برای واژه‌های واقعاً پرریسک استفاده می‌شود.
- timeline قابل‌فهم است، ولی prompt به هزار rule متناقض تبدیل نمی‌شود.

### Anti-pattern

Over-engineering زیاد می‌تواند خودش باعث segmentation مصنوعی، عجله یا restart شود.

Rule:

> Start from a proven simple architecture; add only the minimum constraints required by the observed failure.

---

# 7. User reference image — Duck.ai

برای Duck.ai چند portrait مقایسه شد.

## Video reference — قفل‌شده

Portrait اول:

- نگاه مستقیم به دوربین
- black suit / black shirt / tie
- executive chair
- office shelves
- serious authoritative expression

دلیل انتخاب:

- مناسب talking-head Reel
- direct eye contact
- سازگار با aggressive hook
- authority / trust

## Cover reference — آخرین تصمیم

در ادامه user صریحاً خواست **همان portrait اول** برای cover Duck.ai هم استفاده شود.

پس تصمیم جدید supersede می‌کند انتخاب موقت portrait دوم برای cover را.

Canonical current choice:

- Video: portrait اول
- Cover: portrait اول

---

# 8. Cover design learnings — Duck.ai

User نمونه cover Z.ai را از نظر visual language دوست داشت ولی گفت:

> از طرح نمونه ایده بگیر، دقیقاً clone نکن.

### Direction موفق

- dark navy / black lower gradient
- cyan / turquoise accent
- large Persian headline blocks
- rounded 3D cards / pills
- small support icons
- subject clearly visible در نیمه بالا
- tool logo در پایین
- strong hierarchy

### Duck.ai headline direction

- top hook: `پول اشتراک نده`
- main benefit: `چند هوش مصنوعی رایگان یه جا!`
- support line: `بدون ثبت‌نام`
- reveal: Duck.ai logo / duck mark

### Important

Cover باید از نمونه inspiration بگیرد، نه اینکه text و layout محصول قبلی را copy کند.

---

# 9. Caption rules

Caption نهایی Duck.ai به‌جای اغراق، کاربرد واقعی را توضیح می‌دهد:

- اسم ابزار: Duck.ai
- چند مدل AI در یک محیط
- استفاده برای سؤال‌وجواب، متن، ایده، خلاصه، برنامه‌نویسی، تحقیق
- image generation
- برای شروع حساب کاربری لازم نیست
- free tier ممکن است usage limit داشته باشد

### Truth rule

`رایگان` را می‌توان گفت اگر free tier واقعی وجود دارد.

`نامحدود` را بدون evidence نباید گفت.

---

# 10. RTL / LTR rule — فارسی و انگلیسی

User صریحاً خواست جمله‌هایی که Persian + English را باهم قاطی می‌کنند ساخته نشوند چون layout در Instagram/Chat ممکن است جابه‌جا یا برعکس شود.

### Rule

برای comment replies و copy عمومی:

- یا جمله کامل فارسی باشد؛
- یا جمله کامل انگلیسی باشد؛
- در جمله فارسی، اسم ابزار در صورت نیاز به شکل فارسی transliterate شود.

برای Duck.ai در replyهای فارسی:

`داک ای‌آی`

نمونه:

`اسم ابزار داک ای‌آی هست 🔥 آموزش استفاده رو کامل توی کپشن گذاشتم.`

---

# 11. Comment reply rotation

برای keyword `همه` چند reply چرخشی استفاده شود تا پاسخ‌ها یکسان نباشند.

نمونه‌های پذیرفته‌شده:

- `اسم ابزار داک ای‌آی هست 🔥 آموزش استفاده رو کامل توی کپشن گذاشتم.`
- `پیداش کردی 😎 اسمش داک ای‌آی هست؛ مراحل استفاده داخل کپشنه.`
- `این همون ابزار داک ای‌آی هست 👌 بدون ثبت‌نام می‌تونی شروع کنی.`
- `اسمش داک ای‌آی هست ⚡️ توضیحات کامل و روش استفاده رو توی کپشن نوشتم.`

Rule:

- reply ثابت زیر همه commentها paste نشود.
- 6–12 variant کوتاه داشته باشیم.
- متن فارسی خالص برای جلوگیری از RTL/LTR preferred است.

---

# 12. Credit-aware production rule

در این cycle user گفت credit کم است و فرصت آزمون‌وخطا ندارد.

وقتی این constraint فعال است:

- یک best production prompt بده.
- variantهای render را پیشنهاد نده مگر ضرورت واقعی.
- قبل از render prompt را self-audit کن.
- dialogue density را کاهش بده.
- risky pronunciation را simplify کن.
- reference identity را دقیق lock کن.
- after-render QA باید practical باشد: ایراد جزئی غیرقابل‌تشخیص برای مخاطب، دلیل render دوباره نیست.

---

# 13. Approved / Proven patterns from this cycle

## A — Successful skincare speech architecture

User یک prompt skincare موفق ارائه کرد که این ویژگی‌ها را داشت:

- 10s exact
- one continuous primary shot
- reference character lock
- simple scene + camera definition
- performance blocks
- exact spoken dialogue
- pronunciation constraints فقط برای واژه‌های مشکل‌دار
- strict no-repeat / no-stutter
- no generated text

Status: `APPROVED-PATTERN`

## B — Z.ai no-reference creator architecture

- fixed fictional character identity
- real silence between every sentence
- aggressive hook + simple benefit + short benefit + CTA
- full silent end hold
- exact spoken Persian
- targeted `میخوایش` lock

Status: `APPROVED-RENDER / APPROVED-PATTERN`

## C — Duck.ai reference-image talking creator

- same user identity from provided portrait
- black professional styling
- simple office
- controlled hook
- split benefit into short sentences
- one continuous CTA without internal punctuation
- product hidden in video

Status: `APPROVED-RENDER`

---

# 14. Default checklist for next AI-tool Reel

Before script:

- [ ] ابزار واقعاً ارزش Reel دارد؟
- [ ] claimهای رایگان / محدودیت verify شده‌اند؟
- [ ] hook benefit-first و تهاجمی است؟
- [ ] اسم ابزار باید داخل video مخفی بماند یا reveal شود؟

Before prompt:

- [ ] dialogue چهار block یا کمتر
- [ ] هیچ block مجبور به machine-gun delivery نیست
- [ ] punctuation CTA باعث split ناخواسته نمی‌شود
- [ ] risky words ساده‌سازی شده‌اند
- [ ] one continuous shot مگر دلیل قوی برای cut وجود دارد
- [ ] reference mode درست است
- [ ] character identity lock کافی است
- [ ] no generated text
- [ ] product reveal rule روشن است

Before spending credit:

- [ ] `high energy != fast speech`
- [ ] each word once
- [ ] no restart / no stutter
- [ ] exact dialogue یک authoritative version دارد
- [ ] final CTA یک phrase طبیعی است
- [ ] success checklist وجود دارد

After render:

- [ ] مخاطب عادی artifact صوتی واضح می‌شنود؟
- [ ] repetition / cut / stutter هست؟
- [ ] چهره drift کرده؟
- [ ] hook قابل‌فهم است؟
- [ ] اگر فقط timing چند دهم ثانیه فرق دارد ولی طبیعی است، render دوباره نکن.

---

# 15. Supersession rules

تصمیم‌های جدید این cycle که باید روی ruleهای قدیمی override شوند:

1. Duck cover: portrait اول جایگزین انتخاب موقت portrait دوم شد.
2. Duck hook spoken-safe: `حتی ثبت نام هم نکن` جایگزین `حتی ثبت‌نامم نکن` شد.
3. Duck CTA: `اگه میخوایش همه رو کامنت کن.` جایگزین `اگه میخوایش؟ همه رو کامنت کن.` شد.
4. Keyword emphasis در CTA اگر باعث restart می‌شود حذف شود.
5. Prompt simplicity از افزودن constraintهای بی‌پایان اولویت بالاتری دارد.

---

# 16. Source-of-truth split

- این فایل: تصمیم‌ها، failureها، corrections، UX/content learnings.
- `11_prompt-libraries/flow-reels-approved-ai-tools-2026-09-03.md`: prompt baselineهای production-ready همین cycle.
- `11_prompt-libraries/flow-reels-approved-prompts.md`: کتابخانه قبلی Flow/Reels و baselineهای Rose / Gemini Live / continuity.

اگر conflict وجود داشت، rule جدیدتر با evidence مشخص supersede می‌کند، ولی تاریخچه حذف نمی‌شود.
