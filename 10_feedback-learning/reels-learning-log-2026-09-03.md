# Reels Learning Log — 2026-09-03

این log، تجربه‌ها و تصمیم‌های تأییدشده از چرخه ساخت Reelهای اخیر با Google Flow / Gemini را ثبت می‌کند. هدف: جلوگیری از تکرار failureها و کاهش هزینهٔ render.

## Scope

- talking-character Reels
- Rose identity
- Google Flow / Gemini video prompting
- Persian speech
- multi-clip continuity
- cover design
- Telegram funnel
- tutorial PDF workflow

این log performance Instagram را فقط وقتی ثبت می‌کند که دادهٔ واقعی user موجود باشد؛ هیچ metric حدسی اضافه نمی‌شود.

---

# 1. کارهایی که انجام شد

## Gemini Live / skeptical investigator Reel

- concept: هوک شبه‌هشدار + clarification واقعی
- C01 در 8 ثانیه با speech blockهای کوتاه و silenceهای واقعی ساخته شد.
- C01 مورد قبول قرار گرفت و baseline موفق prompt architecture شد.
- C02 ابتدا از نظر reaction ضعیف بود؛ `نترس!` به emotional reaction و chuckle نیاز داشت.
- تلفظ ترکیب `لایوئه / لایوه` ناپایدار بود؛ تصمیم: foreign product name را مستقل بگوییم یا suffix را حذف کنیم.

### Learning

Prompt فقط dialogue نیست؛ **acting timeline** به‌اندازه متن مهم است.

---

## Google Flow long-video tutorial teaser

هدف نهایی Reel:

- general audience بفهمد موضوع ساخت Reel/video است؛
- limitation کلیپ کوتاه را بفهمد؛
- promise یک ویدیوی حدود 1 دقیقه‌ای بگیرد؛
- برای آموزش کامل به Telegram هدایت شود.

### Script direction نهایی

`برای پیجت ریلز می‌خوای بسازی؟ → ولی گوگل فلو فقط ده ثانیه ویدیو می‌ده؟ → بیا یاد بدم چطور یک‌دقیقه‌ای بسازی → آموزش کامل تو کانال تلگرام`

### مهم‌ترین تصمیم

Reel **خودش method را آموزش نمی‌دهد**.

روش:

- final frame
- next clip
- continuity
- InShot

همه به tutorial منتقل شدند.

### Learning

Teaser Reel باید curiosity gap را حفظ کند. اگر method داخل 10 ثانیه توضیح داده شود، هم dialogue شلوغ می‌شود و هم دلیل رفتن به Telegram کم می‌شود.

---

## Telegram funnel asset

- CTA spoken: آموزش کامل در کانال Telegram.
- gesture: finger points down.
- username به‌صورت edit overlay اضافه می‌شود، نه generated text داخل Flow.
- Telegram handle مورد استفاده: `t.me/asdev_ai` / `@asdev_ai`.

### Learning

CTA gesture باید از ابتدا در prompt composition لحاظ شود؛ lower-center باید خالی بماند.

---

## Telegram tutorial PDF

آموزش ساخته‌شده:

- سناریوی 60 ثانیه‌ای → 6 بخش تقریباً 10 ثانیه‌ای
- ساخت C01
- گرفتن best clean final frame
- استفاده از frame قبلی برای C02
- تکرار تا C06
- continuity prompt
- assemble در InShot
- trim duplicate frames
- subtitle/music بعد از assemble

### Learning

این workflow یک **chained-video method** است، نه claim ساخت direct native 60s clip.

---

# 2. چیزهایی که خوب جواب دادند

## A. Absolute Audio Timeline

موفق‌ترین تغییر prompt:

- start/end دقیق هر speech block
- silence duration دقیق
- instruction صریح `Never begin a speech block early`
- instruction صریح `Do not fill silence with speech`

### Strength

به model اجازه نمی‌دهد برای optimize کردن duration همه جملات را پشت‌سرهم بگوید.

---

## B. Facial Acting During Silence

در pause فقط `NO SPEECH` کافی نیست. باید micro-action تعریف شود:

- eye contact
- eyebrow raise
- squint
- head tilt
- glance to phone
- half-smile
- breathing

### Strength

Silence به dead air تبدیل نمی‌شود؛ suspense / personality می‌سازد.

---

## C. Exact Spoken Persian + targeted diacritics

اعراب فقط روی واژه‌های پرریسک:

- `گوگِل`
- `فِلو`
- `جِمِنای`
- `تِلِگرام`
- `یِک‌دَقیقه‌ای`

### Strength

خوانش را راهنمایی می‌کند بدون اینکه کل متن مصنوعی و سخت‌خوان شود.

---

## D. Separate product name from risky suffixes

وقتی `Live + ـه` بد تلفظ شد، sentence structure عوض شد.

### Strength

به‌جای fighting phonetics، syntax ساده‌تر شد.

---

## E. Character Identity Lock

برای Rose فقط `pink/blue hair` کافی نیست. pattern باید دقیق باشد:

`dark roots + magenta outer/front + blue underlayer`

### Strength

hair drift کمتر و identity قابل‌شناسایی‌تر می‌شود.

---

## F. Independent prompt when no reference should be uploaded

وقتی prompt عبارت `provided reference image` داشت، Gemini image request کرد.

### Fix

اگر user reference نمی‌دهد:

- appearance self-contained نوشته شود؛
- هر mention از provided/reference image حذف شود.

---

# 3. Failureها و corrective rules

## Failure 01 — Dialogue overload

### Symptom

- رگباری
- robotic
- pauses حذف‌شده
- pronunciation ضعیف

### Root cause

هدف‌گذاری بیش از حد برای یک 8/10s Reel.

### Rule

Script را کم کن؛ سرعت را زیاد نکن.

---

## Failure 02 — Teaching inside teaser

### Symptom

Reel هم hook، هم method، هم CTA را می‌خواهد در 10 ثانیه جا دهد.

### Rule

`Problem → Promise → Destination`

Method در Telegram / PDF.

---

## Failure 03 — Technical naming before user benefit

### Symptom

اسم مدل برای audience عمومی نامفهوم یا بدتلفظ است.

### Rule

Outcome first. Technical model name فقط اگر برای story لازم است.

---

## Failure 04 — Cover visually strong but semantically unclear

### Symptom

طرح جذاب است ولی مخاطب عمومی نمی‌فهمد Reel درباره چیست.

### Rule

Headline باید بدون دیدن Reel قابل‌فهم باشد.

Final cover direction accepted:

- `با هوش مصنوعی گوگل فلو`
- **`ویدیوی بلند بساز`** — بزرگ‌ترین headline
- `آموزش در کانال تلگرام` — secondary
- Rose on cover

---

## Failure 05 — Emotionally flat reaction

### Example

`نترس!` بدون smile/chuckle/relaxation از نظر acting ضعیف بود.

### Rule

Emotion words باید corresponding visual reaction داشته باشند.

---

# 4. Cover Learnings

## General Audience Test

قبل از قبول cover بپرس:

> اگر کسی Flow یا اسم مدل را نشناسد، در یک ثانیه می‌فهمد benefit چیست؟

اگر جواب `نه` است، headline باید rewrite شود.

## Accepted visual direction

- dark / black / deep navy base
- electric blue / purple neon
- yellow high-contrast key phrase
- 3D Persian headline
- clear hierarchy
- Rose visible for character-led Reel
- Telegram CTA secondary, نه dominant

## Headline hierarchy

1. context کوچک‌تر
2. outcome بسیار بزرگ
3. CTA کوچک‌تر

Example:

`با هوش مصنوعی گوگل فلو`

`ویدیوی بلند بساز`

`آموزش در کانال تلگرام`

---

# 5. Telegram Education Workflow

Reel → Cover → Caption → Telegram CTA overlay → Telegram post → PDF

### Reel

فقط promise.

### Caption

context مختصر؛ method کامل لو نرود.

### Telegram post

value proposition + PDF download.

### PDF

step-by-step + copy-ready prompt blocks.

### Strength

Instagram برای reach / curiosity؛ Telegram برای depth / retention / owned audience.

---

# 6. Conditional Cost Rule

User در این cycle صریحاً گفت امکان پرداخت/credit بیشتر برای آزمون‌وخطا ندارد.

### Classification

conditional workflow rule، نه فرض دائمی درباره budget.

### Rule

وقتی user می‌گوید credit محدود است:

- فقط یک best prompt بده؛
- variant تستی پیشنهاد نده؛
- قبل از final، dialogue density و timing را self-audit کن؛
- reference requirements را دوباره بررسی کن؛
- pronunciation-risk words را fix کن؛
- final success checklist داخل prompt قرار بده.

---

# 7. Approved Prompt Baselines

جزئیات exact در:

`11_prompt-libraries/flow-reels-approved-prompts.md`

Canonical approved baselines در زمان ثبت این log:

- P-001 Timed Speech + Real Silence Contract
- P-002 Gemini Live C01 8s
- P-003 Rose Identity / Hair Lock
- P-004 One-Minute Tutorial Teaser 10s
- P-005 Chained Clip Continuity Block

Prompt شخصیت `Fatemeh` در انتهای گفتگو فقط برای test نوشته شد و تا وقتی output صریحاً approve نشود، **approved baseline نیست**.

---

# 8. Default Future Reel Checklist

قبل از prompt:

- [ ] audience مشخص
- [ ] hook عمومی و قابل‌فهم
- [ ] one promise
- [ ] one CTA
- [ ] technical jargon حذف‌شده مگر ضروری

قبل از render:

- [ ] dialogue کوتاه است
- [ ] speech blocks زمان‌بندی شده‌اند
- [ ] real silence وجود دارد
- [ ] pronunciation locks تعریف شده‌اند
- [ ] identity lock کامل است
- [ ] wardrobe self-contained است اگر reference نداریم
- [ ] camera ثابت است
- [ ] generated text ممنوع است
- [ ] CTA gesture دقیق است

بعد از render:

- [ ] video QA قبل از cover
- [ ] cover headline general-audience test پاس می‌کند
- [ ] caption با Reel تکراری نیست
- [ ] Telegram/PDF فقط اگر واقعاً آماده است promise شود

---

# 9. Promotion / Supersession

این log تاریخچه است. اگر evidence جدید یک rule را تغییر داد:

- rule قبلی حذف نشود؛
- status آن `superseded` شود؛
- نسخه جدید با provenance ثبت شود.

هدف این سیستم حفظ **reasoning history بدون تبدیل هر approval محلی به قانون جهانی** است.
