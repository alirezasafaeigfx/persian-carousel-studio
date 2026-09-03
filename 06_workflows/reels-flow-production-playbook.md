# Reels + Google Flow Production Playbook

این سند حافظهٔ اجرایی ساخت Reelهای ASDEV با Google Flow / Gemini است. هدفش کم‌کردن آزمون‌وخطا، جلوگیری از فراموشی تصمیم‌ها، و تبدیل تجربه‌های موفق به workflow قابل‌تکرار است.

## اصل شماره ۱ — اعتبار Flow را نسوزان

وقتی امکان تست چندباره وجود ندارد، prompt باید با ذهنیت **one-shot production** نوشته شود:

`short script → exact timing → real silence → identity lock → pronunciation lock → gesture lock → no generated text`

نسخه‌های متعدد A/B فقط وقتی مجازند که کاربر صریحاً اعتبار کافی برای تست داشته باشد.

## فرمول اصلی Reel کوتاه

برای Reelهای 8 تا 10 ثانیه‌ای، بهترین ساختار فعلی:

`Hook / Problem → real pause → Promise / Payoff → real pause → one CTA`

قواعد:

- Dialogue را به یک پاراگراف پیوسته تبدیل نکن.
- هر speech block زمان شروع/پایان مشخص داشته باشد.
- بین blockها سکوت واقعی تعریف شود.
- اگر جمله زود تمام شد، مدل باید صبر کند؛ نباید block بعدی را زود شروع کند.
- facial acting در سکوت مهم است.
- CTA فقط یک مورد باشد.
- Reel teaser نباید آموزش کامل را داخل خودش لو بدهد.

## تراکم Dialogue

Rule of thumb:

- در 8 ثانیه: 3 تا 4 phrase کوتاه، نه یک متن بلند.
- در 10 ثانیه: حدود 3 یا 4 speech block کوتاه با pause واقعی.
- اگر برای جا شدن جمله‌ها مجبور به machine-gun delivery می‌شویم، script باید کوتاه شود؛ نه اینکه سرعت voice را بالا ببریم.

## Voice Contract

صدای هدف:

- contemporary Iranian Persian
- creator-native
- human breathing
- changing pitch / speed
- natural hesitation where useful
- real silence

ممنوع:

- robotic cadence
- news presenter
- advertisement narrator
- monotone
- continuous speech at constant speed
- rushing final CTA

## Persian Pronunciation

برای واژه‌هایی که مدل احتمالاً خراب می‌کند، داخل Exact Spoken Persian اعراب‌گذاری حداقلی و هدفمند انجام شود.

نمونه:

- `گوگِل`
- `فِلو`
- `جِمِنای`
- `تِلِگرام`
- `یِک‌دَقیقه‌ای`

اگر یک ترکیب باعث تلفظ بد می‌شود، **ساختار جمله را عوض کن**؛ صرفاً phonetic spelling را پیچیده‌تر نکن.

نمونهٔ موفق: به‌جای چسباندن پسوند فارسی به `Live`، اسم مستقل گفته شود: `جِمِنای لایو`.

## Rose — Canonical Identity

Rose باید در Reelهای مربوط به شخصیت ثابت، فوراً قابل‌شناسایی بماند:

- Persian woman ~25
- youthful oval face
- warm light-to-medium skin
- dark brown almond eyes
- full dark eyebrows
- slim nose + subtle nose piercing
- round thin black eyeglasses
- chin-length bob
- very dark / near-black roots
- vivid hot-magenta front + outer sections
- sapphire / electric-blue underneath

### Hair Lock

الگوی رنگ مو نباید drift کند:

`dark roots + hot-magenta front/outer + sapphire-blue underlayer`

ممنوع:

- fully pink
- fully purple
- fully blue
- long hair
- ponytail
- removing glasses
- face redesign

## Wardrobe Rule

لباس می‌تواند برای هر Reel تغییر کند، ولی identity تغییر نمی‌کند.

برای prompt بدون reference image، لباس را کامل در متن تعریف کن. اگر کاربر نمی‌خواهد عکس reference به Flow بدهد، هر عبارت مثل `provided reference image` باید حذف شود.

## Camera Rule

Default برای talking Reel:

- vertical 9:16
- stable medium / medium-close shot
- camera essentially locked
- no orbit
- no whip pan
- no dramatic zoom
- no unnecessary shot changes

Gesture یا فضای ادیت از قبل در composition دیده شود. مثال: اگر آیدی تلگرام باید پایین قرار بگیرد، lower-center space خالی و finger direction دقیق تعریف شود.

## Telegram Funnel Pattern

برای Reelهایی که هدفشان انتقال به Telegram است:

1. Reel فقط مشکل و promise را می‌گوید.
2. روش کامل داخل Reel آموزش داده نمی‌شود.
3. پایان: `آموزش کامل ... کانال تلگرام`.
4. هنگام گفتن `کانال تلگرام` انگشت به پایین اشاره کند.
5. 0.5 تا 0.8 ثانیه ending hold بدون speech برای ادیت آیدی.
6. username / Telegram logo / arrow توسط مدل تولید نشود؛ در ادیت اضافه شود.

## General-Audience Cover Rule

Cover باید بدون دانستن نام ابزار هم قابل‌فهم باشد.

بد:

- headline فنی یا اسم مدل به‌تنهایی
- عبارتی که فقط کاربر Flow معنی آن را بفهمد

بهتر:

- outcome-first
- number / contrast
- plain-language benefit

نمونه‌های موفق/تأییدشده در این session:

- `ویدیوی ۱۰ ثانیه‌ای رو ۱ دقیقه کن!`
- `با هوش مصنوعی گوگل فلو` + `ویدیوی بلند بساز` + `آموزش در کانال تلگرام`

Design direction پذیرفته‌شده:

- neon blue / purple
- black / deep navy background
- yellow high-contrast payoff
- large 3D Persian typography
- Rose visible on cover when character-led
- Telegram visual language only as secondary CTA

## Long Video with Flow — Chained Continuity Method

برای ساخت حدود 30 یا 60 ثانیه:

`10s clip → best clean final frame → next clip using that frame → repeat → assemble in InShot`

برای 1 دقیقه:

`C01 → frame → C02 → frame → C03 → frame → C04 → frame → C05 → frame → C06`

### مهم

این workflow به معنی direct native 60-second generation نیست. ویدیوی نهایی از چند clip کوتاه ساخته می‌شود.

### انتخاب final frame

آخرین frame فنی الزاماً بهترین reference نیست. فریم نزدیک پایان را انتخاب کن که:

- face sharp باشد
- blink خراب نداشته باشد
- hands سالم باشند
- motion blur شدید نباشد
- body pose واضح و قابل‌ادامه باشد

### Continuity priority

در clip بعدی preserve شود:

- identity / face
- exact hairstyle + hair colors
- wardrobe
- body proportions
- environment
- lighting
- camera height / angle / distance
- framing
- starting body orientation

زنجیره باید مرحله‌ای باشد:

`1 → 2 → 3 → 4 → ...`

برای clip 3 دوباره frame clip 1 را استفاده نکن.

## Editing in InShot

- ابتدا Hard Cut را امتحان کن.
- اگر first frame کلیپ بعدی duplicate است، چند frame trim شود.
- Transition شلوغ ممنوع؛ در صورت نیاز dissolve بسیار کوتاه.
- یک music track واحد روی timeline نهایی continuity صوتی را بهتر می‌کند.
- subtitle بعد از assemble کامل اضافه شود.

## Reel QA Gate

قبل از قبول خروجی:

### Visual
- [ ] identity ثابت است
- [ ] hair pattern ثابت است
- [ ] wardrobe درست است
- [ ] hands / face glitch واضح ندارد
- [ ] camera بی‌دلیل حرکت نکرده

### Speech
- [ ] exact dialogue رعایت شده
- [ ] مکث‌ها واقعی‌اند
- [ ] جمله‌ها رگباری نیستند
- [ ] واژه‌های حساس درست تلفظ شده‌اند
- [ ] extra phrase / CTA اضافه نشده

### CTA
- [ ] فقط یک CTA
- [ ] gesture دقیق و قابل‌استفاده در edit
- [ ] ending hold کافی

### Text
- [ ] no generated subtitles
- [ ] no random Persian/English text
- [ ] no fake UI

## Failure Patterns Learned

1. **Dialogue too dense** → robotic / rushed result.
2. **Prompt says reference image when none should be provided** → Gemini asks for image.
3. **Technical model name in consumer hook** → confusion + pronunciation risk.
4. **Teaching the method inside teaser Reel** → kills curiosity gap.
5. **Unclear cover headline** → visual quality may be high but general audience cannot understand topic.
6. **Neutral acting on emotional line** → dialogue may be technically correct but Reel feels dead.
7. **Suffix attached to foreign product term** → pronunciation errors can increase.

## Default Decision Order for Future Reels

1. Define audience-visible outcome/problem.
2. Write the shortest possible Persian dialogue.
3. Remove technical jargon that is not needed in speech.
4. Mark pronunciation-risk words.
5. Split into timed speech blocks.
6. Add real silence.
7. Lock character identity.
8. Define wardrobe/environment/camera.
9. Define one specific gesture if needed.
10. Add strict negatives.
11. Render once.
12. QA actual video before designing cover.
13. Cover = outcome-first, readable to general audience.
14. Caption / pinned comment / Telegram content carry the full explanation.

## Source-of-Truth rule

Approved prompt structures live in:

`11_prompt-libraries/flow-reels-approved-prompts.md`

Session learnings and provenance live in:

`10_feedback-learning/reels-learning-log-2026-09-03.md`
