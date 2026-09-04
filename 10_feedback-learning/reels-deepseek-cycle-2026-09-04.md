# DeepSeek Reel Production Cycle — 2026-09-04

این سند حافظهٔ اجرایی چرخهٔ DeepSeek برای ASDEV است. هدف: ثبت تصمیم‌ها، خطاها، اصلاحات، داده‌های واقعی Instagram و baseline نهایی تا Reelهای بعدی از همین evidence شروع شوند و credit روی آزمون‌وخطای تکراری نسوزد.

> Status: `APPROVED-RENDER` برای ویدیوی نهایی DeepSeek + `APPROVED-VISUAL-DIRECTION` برای کاور + `WORKFLOW-LEARNING` برای تحلیل سه Reel.

---

## 1) داده‌های واقعی سه Reel که قبل از DeepSeek تحلیل شد

### Reel A — Copilot / «دیگه پول نده، رایگان شد!»
- Views: 20,943
- Viewers: 13,248
- Average watch time: 8s
- Follows: 422
- Non-followers: 94.3%
- Comments: 1,474
- Shares: 149
- Saves: 315
- Skip rate: 44.3%
- Comment rate: ~10.7%

### Reel B — Chat / image utility cover
- Views: 39,753
- Viewers: 29,002
- Average watch time: 6s
- Follows: 689
- Non-followers: 97.1%
- Likes: 602
- Comments: 1,664
- Shares: 683
- Saves: 926
- Profile visits: 585
- Bio link taps: 449
- Skip rate: 49.3%
- Share rate: 2.4%
- Save rate: 3.2%
- Comment rate: 5.8%
- Top sources: Reels 62.2%, Explore 27.6%

### Reel C — «همه‌شون تو یه برنامه!»
- Views: 11,807
- Viewers: 7,990
- Average watch time: 7s
- Follows: 208
- Non-followers: 90.3%
- Likes: 223
- Comments: 721
- Shares: 125
- Saves: 256
- Profile visits: 138
- Bio link taps: 40
- Skip rate: 41.8% — بهترین بین این سه
- Share rate: 1.6%
- Save rate: 3.2%
- Comment rate: 9.1%
- Top sources: Reels 68.4%, Explore 20.1%

### Audience signal
در سه Reel، بخش اصلی مخاطب بزرگسال بود. در Reel سوم:
- 25–34: 25.3%
- 35–44: 26.6%
- 45–54: 21.8%
- 25–54 total: 73.7%

### Strategic conclusions
1. KPI اصلی این سری فقط Like نیست؛ `Share + Save + Comment + Follow + Watch` مهم‌ترند.
2. CTA تک‌کلمه‌ای کامنت به‌وضوح جواب می‌دهد؛ آن را حفظ کن.
3. Shareability باید از خود claim بیاید، نه CTA دوم.
4. بزرگ‌ترین فرصت بهبود در 0–2s است.
5. `START EARLY != SPEAK FAST`.
6. 1s سکوت ابتدای Reel برای discovery گران است؛ micro lead-in حدود 0.2–0.3s بهتر است.
7. وسط Reel باید lean بماند؛ Hook → یک claim قوی → CTA.
8. برای audience فعلی، hookهای هزینه/دسترسی/کاربرد از hype عمومی قوی‌ترند.

---

## 2) انتخاب DeepSeek و زاویهٔ محتوا

DeepSeek برای Reel بعدی انتخاب شد چون با intent مخاطب ASDEV هم‌راستا بود: رایگان، کاربردی، و موضوع دسترسی برای کاربران ایرانی.

### Keyword CTA
`واقعی`

### Funnel
- اسم DeepSeek در spoken video گفته نشود.
- Reveal روی cover / caption / comment reply.
- فقط یک CTA داخل ویدیو.

---

## 3) Script evolution و نسخهٔ نهایی render پذیرفته‌شده

نسخهٔ اولیهٔ concept:

`رایگان واقعی میخوای؟`

`حتی وقتی خیلی از هوش مصنوعی‌ها در دسترس نبودن، این یکی هنوز کار می‌کرد!`

`اگه میخوایش واقعی رو کامنت کن.`

در جریان render و اصلاح pronunciation، جملهٔ میانی به نسخهٔ production زیر تبدیل شد و ویدیوی نهایی با آن پذیرفته شد:

```text
«رایگان واقعی میخوای؟»

[REAL SILENCE]

«این هوش مصنوعی حتی وقتی اینترنت جهانی قطع بشه، بازم در دسترسه.»

[REAL SILENCE]

«اگه میخوایش، واقعی رو کامنت کن.»
```

### Factual-risk note — مهم
عبارت «حتی وقتی اینترنت جهانی قطع بشه، بازم در دسترسه» یک claim وابسته به شرایط شبکه/زمان/اپراتور است و نباید به‌عنوان حقیقت دائمی یا universal baseline برای Reelهای آینده reuse شود. قبل از انتشار مجدد یا استفاده در محتوای دیگر باید دوباره verify شود. از claimهای مطلق مثل «همیشه»، «برای همه»، «هیچوقت قطع نمی‌شود» اجتناب شود.

---

## 4) خطاهای مهم Flow و اصلاحات

### Failure A — character مرد / خروجی مصنوعی
نسخهٔ اولیه با شخصیت مرد رسمی/اجرایی از نظر user بیش از حد مصنوعی بود:
- پوست و نور تبلیغاتی
- executive/corporate feeling
- mouth movement بزرگ‌تر از طبیعی
- facial acting نمایشی

### Fix
بازگشت به Lia و creator-style organic video.

Rule:
> برای talking Reels این سری، `organic creator + natural imperfections controlled + restrained mouth movement` از executive commercial look طبیعی‌تر است.

---

### Failure B — Lia بیش از حد skin-textured
وقتی prompt روی pores / imperfections بیش از حد تأکید کرد، مدل جوش و کک‌ومک اضافه کرد.

### Fix skin contract
Target:
`clear + healthy + natural + softly refined`

Avoid:
- visible acne
- prominent freckles
- heavy texture
- exaggerated pores
- waxy / plastic skin

Rule:
> natural skin ≠ deliberately blemished skin.

---

### Failure C — «هوش مصنوعی» بد تلفظ شد
Symptom:
`هوش مصنعی`

### Fix
Targeted pronunciation lock:
- exact phrase: `هوش مصنوعی`
- do not drop the «و» sound inside `مصنوعی`
- do not over-articulate
- exact phrase once

Higher-order rule:
> اگر واژه واقعاً failure نشان داده، lock هدفمند اضافه کن؛ همهٔ prompt را phonetic نکن.

---

### Failure D — «نت جهانی» به شکل «نَت جهانی» گفته شد
این خطا چند بار تکرار شد.

### Wrong corrective attempt
تلاش برای نگه‌داشتن واژهٔ `نت` و فقط نوشتن دستور pronunciation ریسک را کم نکرد.

### Final fix
spoken phrase از:
`نت جهانی`

به:
`اینترنت جهانی`

تغییر کرد.

Rule:
> وقتی یک token کوتاه در TTS repeatedly wrong است، syntax را عوض کن؛ با phonetic over-control نجنگ.

---

### Failure E — visual cut / reset وسط ویدیو
در یک render، حدود 3.88s continuity شکست و چهره/مو/pose reset شد؛ حس jump cut ایجاد کرد.

### Root cause
`one continuous primary shot` به‌تنهایی کافی نبود و push-in / performance segmentation می‌توانست shot boundary بسازد.

### Final fix
Prompt نهایی صریحاً این قرارداد را قفل کرد:
- `ONE SINGLE UNINTERRUPTED 10-SECOND RECORDING`
- not multiple shots
- no hidden cuts
- no transition
- no pose reset
- no background reset
- camera completely locked
- silent pauses must happen inside the SAME TAKE
- critical continuity window 3.50–4.30s

Rule:
> اگر Flow وسط pause یا speech block shot reset می‌زند، continuity را به‌صورت frame-to-frame physical continuation تعریف کن؛ فقط عبارت `one continuous shot` کافی نیست.

---

## 5) Lia — هویت نهایی DeepSeek Reel

ویدیوی پذیرفته‌شده `deepseek-free.mp4`، 10s، 1080×1920.

First-frame identity برای cover و continuity:
- زن جوان ایرانی
- long light-brown / warm brunette hair
- black rounded-square glasses
- hazel/warm brown eyes
- subtle nose piercing
- cream/off-white knit top
- clear natural skin
- warm realistic home-office / workspace
- direct eye contact

### Cover rule
برای کاور DeepSeek از **فریم اول خود Reel نهایی** به‌عنوان identity anchor استفاده شود؛ نه یک Lia مشابه یا redesign شده.

---

## 6) Timing / delivery نهایی

Production contract:
- 0.00–0.30: micro visual lead-in, no speech
- Hook بلافاصله بعدش شروع شود
- Hook energetic ولی نه سریع
- real silence بین blocks
- CTA یک phrase طبیعی
- no filler during silence
- no mouthing next line
- camera locked

Canonical principle:

`START EARLY DOES NOT MEAN SPEAK FAST.`

و:

`HIGH ENERGY DOES NOT MEAN FAST SPEECH.`

---

## 7) Cover direction — پذیرفته‌شده

User یک reference پوستر با motion-blurred papers / dark cinematic composition داد و خواست فقط از ایده استفاده شود، نه clone.

DeepSeek cover direction:
- 9:16
- dark navy / black cinematic background
- motion-blurred floating UI/paper elements around edges
- orange / electric-blue accents
- Lia from first frame of final Reel as identity source
- large Persian hierarchy
- DeepSeek reveal near bottom
- ASDEV branding subtle

Accepted copy direction used in visual exploration:
- `رایگان واقعی`
- main value line around `هوش مصنوعی ... ایرانی‌ها`
- DeepSeek logo/name

### Factual-risk note برای cover
هر عبارت مثل `مخصوص ایرانی‌ها` یا `حتی با قطع نت/اینترنت جهانی` باید پیش از reuse یا publish مجدد از نظر factual accuracy دوباره بررسی شود. visual approval به‌معنای factual permanence نیست.

---

## 8) Caption pack — ساختار نهایی

Caption final شامل:
- reveal: DeepSeek
- کاربردها: پرسش/متن/ایده/فایل/جست‌وجو و productivity
- نصب Android از Google Play با تأکید بر official publisher
- نصب iOS از App Store
- استفاده از نسخه وب رسمی
- مثال promptهای ساده
- security caution برای اطلاعات حساس
- CTA: کامنت `واقعی`
- Brand signature:

`ASDEV ⚡️`

`هوش مصنوعی رو فقط معرفی نمی‌کنیم؛ کاربرد واقعیش رو نشون می‌دیم.`

Hashtag direction:
`#هوش_مصنوعی #دیپ_سیک #DeepSeek #ابزار_رایگان #ASDEV`

---

## 9) Credit-efficiency policy — از این چرخه قفل شود

1. وقتی visual quality خوب است، فقط failure واقعی را اصلاح کن؛ style را از نو طراحی نکن.
2. هر render باید یک هدف اصلاحی مشخص داشته باشد.
3. قبل از تغییر prompt بپرس: آیا مشکل از syntax است یا constraint؟
4. pronunciation failure → اول sentence simplification / safer token؛ بعد targeted lock.
5. continuity failure → fixed camera + one uninterrupted take + explicit no-reset contract.
6. اختلاف کوچک timing که user از نظر perceptual تأیید کرده، دلیل render مجدد نیست.
7. output accepted by user + no critical artifact = PASS؛ credit برای perfection میلی‌ثانیه‌ای نسوزان.

---

## 10) Reuse checklist برای Reel بعدی

قبل از Generate:
- [ ] script کوتاه و تصویب شده
- [ ] فقط یک claim اصلی
- [ ] factual claim verify شده
- [ ] keyword CTA یک phrase پیوسته
- [ ] 0.2–0.3s visual lead-in
- [ ] targeted pronunciation locks فقط برای demonstrated failures
- [ ] character identity source مشخص
- [ ] camera locked اگر continuity مهم است
- [ ] `ONE UNINTERRUPTED TAKE` در صورت هر سابقهٔ reset
- [ ] no generated text

بعد از Generate:
- [ ] pronunciation QA
- [ ] frame continuity QA خصوصاً اطراف pauseها
- [ ] identity drift QA
- [ ] skin / glasses / hair QA
- [ ] CTA repeat/restart QA
- [ ] اگر PASS است، دیگر render نکن

---

## Final status

DeepSeek final Reel: `APPROVED-RENDER`.

Key new permanent learnings:
1. `نت` repeatedly mispronounced → safer lexical rewrite to `اینترنت`.
2. `one continuous shot` may still reset → use `ONE SINGLE UNINTERRUPTED RECORDING` + locked camera + no-reset contract.
3. natural-skin prompting must avoid over-requesting imperfections.
4. for this series, Lia / organic creator visual language outperformed artificial executive styling perceptually.
5. preserve credit by correcting the observed failure only, not redesigning a visually successful render.
