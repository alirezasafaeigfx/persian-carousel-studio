# Gemini + Google Flow VPN Reel — Production Cycle — 2026-09-08

## Status

`APPROVED-RENDER-DIRECTION` + `PUBLISH-PACK-READY`

این سند تصمیم‌ها، failureها و learningهای چرخه Reel «رفع مشکل دسترسی به جمنای و گوگل فلو» را ثبت می‌کند تا آزمون‌وخطا و مصرف credit در تولیدهای بعدی تکرار نشود.

> نکته: سرویس معرفی‌شده رایگان نیست. یک کانفیگ V2Ray با هزینه اعلام‌شده توسط کاربر: ماهیانه ۳۰۰ هزار تومان. این مبلغ باید قبل از انتشار دوباره بررسی شود اگر قیمت تغییر کرده باشد.

---

## 1. Goal / Audience

هدف Reel:

- pain point عمومی کاربران ایرانی: باز نشدن Gemini و Google Flow؛
- معرفی همان VPN/V2Ray configuration که creator شخصاً استفاده می‌کند؛
- شفافیت کامل درباره پولی بودن سرویس؛
- CTA کامنت برای دریافت اطلاعات.

اصل claim:

- نگوییم برای همه و همه شبکه‌ها تضمینی کار می‌کند؛
- framing به شکل تجربه شخصی: «من با همین ... باز می‌کنم»؛
- رایگان بودن ادعا نشود.

---

## 2. Locked Dialogue

نسخه نهایی:

```text
«رایگان نیست!»

[REAL SILENCE]

«ماهیانه سیصد تومنه.»

[REAL SILENCE]

«ولی من با همین وی‌پی‌ان جِمِنای و گوگل فلو رو باز می‌کنم.»

[REAL SILENCE]

«اگه میخوایش وی‌پی‌ان رو کامنت کن.»
```

### Dialogue decisions

- «ماهی سیصد تومنه» در render به شکل «ماهیه» تلفظ شد؛ با «ماهیانه سیصد تومنه» جایگزین شد.
- Gemini و Google Flow باید داخل spoken dialogue باقی بمانند؛ حذف نام‌ها پیام Reel را مبهم می‌کند.
- «جِمِنای» targeted pronunciation lock است؛ اعراب گسترده روی کل متن ممنوع/نامطلوب است.
- CTA یک phrase پیوسته است و keyword نباید isolate یا repeat شود.

---

## 3. Visual Direction — Approved

کاراکتر نهایی دیگر Rose canonical با bob magenta/blue نیست. Direction بصری جدید:

- fictional adult Iranian/Persian-speaking woman, mid-20s;
- long dark brunette hair;
- deep side part;
- natural polished makeup;
- light silver-gray structured blazer;
- warm beige/taupe fitted top;
- matching elegant trousers;
- metallic bracelet + small elegant earrings;
- premium editorial styling.

Environment:

- dark premium studio;
- vivid magenta / hot-pink illuminated region;
- violet/purple ambience;
- deep black background areas;
- minimal architectural depth;
- no generic beige home office;
- no gaming-room look;
- no fake product UI.

Camera:

- 9:16;
- medium portrait / waist-up;
- ~50mm portrait perspective;
- one continuous take;
- essentially locked camera;
- no cuts, orbit, pan, tilt, dramatic zoom or reset.

---

## 4. Acting Direction — Critical Learning

یک failure مهم در iteration قبلی: ظاهر صحنه/تیپ و body language مصنوعی بود؛ character مثل presenter تبلیغاتی رفتار می‌کرد.

### Rule promoted from this cycle

برای natural creator performance، gesture-by-keyword ننویس.

Use:

```text
Natural spontaneous body language.
Slight asymmetry.
Imperfect human timing.
Small unscripted hand movements.
Natural weight shifts.
Expressions must emerge from the meaning of the sentence, not from keyword-triggered gestures.
Never pose after each sentence.
Never reset the face between speech blocks.
```

Avoid:

- eyebrow raise after every line;
- nod after every line;
- choreographed CTA acting;
- stiff shoulders;
- expression reset between blocks;
- presenter / commercial delivery.

---

## 5. Generated Text / Overlay Failure

Flow در iteration ناموفق با وجود `NO TEXT` چیزهای اضافی روی ویدیو تولید کرد: subtitle/English/Persian text-like overlays و عناصر جعلی.

### Stronger clean-camera contract

```text
The generated video must contain ONLY the photographed physical scene.
Treat the output as CLEAN RAW CAMERA FOOTAGE.
No post-production layer exists.
No typography layer exists.
No social-media template exists.
Every visible pixel must belong to the physical photographed scene.

ABSOLUTELY NO:
subtitles, captions, automatic transcription, Persian text, English text,
labels, stickers, logos, badges, buttons, arrows, UI, fake browser,
VPN interface, Gemini interface, Google Flow interface, readable screen text.
```

Learning: فقط `NO SUBTITLES` کافی نیست؛ output mode را از ابتدا raw camera plate تعریف کن.

---

## 6. Reference Image / Policy Failure

یک reference image برای character/style انتخاب شد، اما Google Flow آن را نپذیرفت. سپس حتی prompt self-contained اولیه با پیام زیر fail شد:

`This prompt might violate our policies about generating prominent people.`

Generation charge نشد.

### Corrective action

- reference image dependency حذف شد؛
- نام شخصیتی که ممکن است identity-specific interpretation بسازد حذف شد؛
- character صریحاً `ENTIRELY FICTIONAL, ORIGINAL ADULT WOMAN` تعریف شد؛
- prompt گفت character نباید real/public/recognizable person را recreate کند؛
- appearance، wardrobe، lighting و environment self-contained شدند.

### New rule

وقتی reference توسط provider به دلیل person/policy gate رد می‌شود:

1. برای دور زدن gate تلاش نکن؛
2. reference dependency را حذف کن؛
3. character را original fictional adult تعریف کن؛
4. visual attributes را به شکل generic/self-contained منتقل کن؛
5. نام/identity lock غیرضروری را حذف کن؛
6. policy failure را با prompt retries متعدد به credit-risk تبدیل نکن.

---

## 7. Timing / Speech Learnings

در iterationهای ضعیف، Flow pauseهای دقیق را نادیده گرفت و جمله‌ها را به هم چسباند.

Ruleهای موجود همچنان معتبرند:

- `DO NOT SPEAK CONTINUOUSLY`؛
- speech blocks کوتاه؛
- real silence؛
- mouth closed during silence؛
- if line finishes early, wait؛
- high energy != fast speech.

اما این cycle یک نکته مهم را دوباره تأیید کرد:

> اگر مدل برای جا دادن dialogue مجبور به compression می‌شود، constraint بیشتر همیشه solution نیست. dialogue density را audit کن.

در این Reel نام Gemini/Google Flow برای semantics ضروری است، بنابراین حذف نام‌ها راه‌حل مناسبی نبود؛ به‌جای آن visual/performance complexity کاهش داده شد.

---

## 8. Final Visual Prompt Direction (No Reference)

Production prompt باید این قراردادها را ترکیب کند:

- completely fictional original adult woman;
- long dark brunette deep-side-part hair;
- silver-gray blazer + beige/taupe top + matching trousers;
- magenta/violet/black premium editorial studio;
- one continuous 10-second take;
- spontaneous natural body language;
- exact locked dialogue;
- real silence between blocks;
- targeted pronunciation only;
- clean raw camera output;
- no typography/UI/overlays;
- no recreation of real/public/recognizable person.

این direction بعد از رد reference image انتخاب شد و باید baseline این Reel باشد.

---

## 9. Cover Copy

دو direction بررسی شد. نسخه قوی‌تر پیشنهادی:

```text
جمنای و گوگل فلو باز نمیشه؟
راه‌حلش اینجاست
وی‌پی‌ان ماهیانه ۳۰۰ تومن
```

Hierarchy:

1. `جمنای و گوگل فلو` / pain point؛
2. `باز نمیشه؟` یا `راه‌حلش اینجاست` به‌عنوان scroll-stop؛
3. `وی‌پی‌ان ماهیانه ۳۰۰ تومن` کوچک‌تر اما کاملاً خوانا.

Transparency rule: قیمت روی cover/caption پنهان نشود.

---

## 10. Caption / Publish Pack

Caption direction:

- شروع با pain point باز نشدن Gemini/Google Flow؛
- توضیح اینکه creator شخصاً با یک V2Ray configuration متصل می‌شود؛
- disclosure واضح: رایگان نیست؛
- قیمت اعلام‌شده: ماهیانه ۳۰۰ هزار تومان؛
- اگر user دنبال VPN رایگان است، صریحاً بگوییم این گزینه مناسب او نیست؛
- framing تجربه شخصی، نه guarantee عمومی؛
- CTA: کامنت «وی‌پی‌ان» برای دریافت اطلاعات.

Suggested signature:

```text
⚡️ ASDEV
هوش مصنوعی رو فقط معرفی نمی‌کنیم؛ کاربرد واقعیش رو نشون می‌دیم.
```

Suggested hashtags:

`#ویپیان #جمنای #گوگل_فلو #هوش_مصنوعی #V2Ray #گوگل_جمنای #ASDEV`

---

## 11. Failure Summary

### F-01 — Over-engineered correction prompt

Symptom: speech/timing still bad despite many constraints.

Learning: adding more instructions can make performance less natural. Protect the approved visual baseline and modify only the failing dimension.

### F-02 — Artificial acting

Symptom: presenter-like face/body language.

Learning: do not script micro-expression for every phrase. Use semantic/spontaneous performance contract.

### F-03 — Random generated text/UI

Symptom: fake captions/English/Persian text and graphics.

Learning: use clean raw camera footage contract; avoid product screens entirely.

### F-04 — Reference-person policy gate

Symptom: Flow rejected generation as possible prominent-person generation.

Learning: remove reference dependency and create a clearly original fictional adult character; never attempt to evade provider policy.

### F-05 — «ماهی» pronunciation

Symptom: rendered as «ماهیه».

Fix: semantic rewrite to `ماهیانه سیصد تومنه.` rather than phonetic fighting.

---

## 12. Reusable Rules Promoted

1. **Transparent paid-service hook:** disclose paid status immediately when it materially affects user expectation.
2. **Personal-experience framing:** for access/VPN claims, prefer «من با همین ...» over universal claims.
3. **Semantic pronunciation fix > phonetic overload:** rewrite unstable words when possible.
4. **Natural acting contract > gesture choreography.**
5. **Clean raw camera contract > simple NO TEXT instruction.**
6. **Reference policy rejection → original fictional self-contained character**, not retry loops.
7. **Do not remove product names when they are necessary for Reel comprehension.**
8. **Price is mutable:** revalidate before reuse/publication.

---

## 13. Publish Readiness

- [x] problem understandable to general Iranian audience
- [x] paid status disclosed
- [x] price stated
- [x] personal-experience framing
- [x] Gemini + Google Flow explicitly named
- [x] CTA keyword defined: `وی‌پی‌ان`
- [x] cover copy prepared
- [x] caption prepared
- [x] no claim of free/unlimited VPN
- [x] reference-image dependency removed after provider rejection
- [x] key failures documented

Final publish status should only become `PUBLISHED` after actual Instagram publication is confirmed.