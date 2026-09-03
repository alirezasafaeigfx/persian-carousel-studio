# Reels Visual Production Cycle — Session Memory — 2026-09-03

این فایل جمع‌بندی انسانی و اجرایی کارهایی است که در این گفت‌وگو روی Reelهای ASDEV انجام شد؛ هدف این است که Reelهای بعدی از baselineهای موفق شروع شوند و خطاهای تکراری، گیج‌شدن بین styleها و فراموشی تصمیم‌ها کم شود.

---

# 1) چه کارهایی انجام دادیم؟

در این چرخه چند نوع deliverable ساختیم و اصلاح کردیم:

- Coverهای حرفه‌ای Reel با typography بزرگ فارسی و hierarchy مشخص.
- Subtitle PNG جداگانه برای dialogue beatها.
- استوری‌های تبلیغاتی/قرعه‌کشی.
- تصویر Telegram برای انتشار همراه آموزش یا برنامه.
- تصویر مناسب Dashboard / Discover سایت بر اساس Cover همان Reel.
- Prompt ویدیوهای Google Flow / Gemini با speech timing، silence، identity lock و CTA.
- اصلاح pronunciation و syntax جمله‌ها برای جلوگیری از تکرار، stutter یا machine-gun speech.
- ساخت visual language متفاوت برای ژانرهای مختلف: AI tools، detective/mystery، skincare، clay/kids، futuristic، website builder.

موضوع‌هایی که روی آن‌ها کار شد یا asset تولید شد شامل:

- Fun AI
- Qwen
- PhotoLab
- Tehran 2120 / future AI image transformation
- Gemini Pro giveaway
- AI Hub / چند هوش مصنوعی در یک برنامه
- Gemini Live / detective-mystery concept
- CapCut
- Picsart
- child / clay-style Reel
- Copilot
- Z.ai / Z Chat website builder
- Duck.ai / چند AI بدون ثبت‌نام
- skincare consultation Reel

---

# 2) مهم‌ترین pattern محتوایی موفق

برای Reelهای کوتاه 8 تا 10 ثانیه‌ای:

`Hook تهاجمی → مکث واقعی → benefit کوتاه → مکث → benefit دوم → CTA کامنت → ending hold`

### چرا جواب داد؟

- audience در ثانیه اول benefit را می‌فهمد.
- speech رگباری نمی‌شود.
- curiosity gap حفظ می‌شود.
- tool name در Reel لازم نیست لو برود.
- CTA فقط یک رفتار از audience می‌خواهد.

### Rule قفل‌شده

اگر متن فقط با سریع‌خوانی جا می‌شود، **متن کوتاه می‌شود؛ سرعت بالا نمی‌رود.**

---

# 3) Voice / Flow — چیزهایی که واقعاً جواب داد

Promptهای موفق section-based بودند:

```text
VIDEO FORMAT
REFERENCE CHARACTER / CHARACTER
SCENE
CAMERA
PERFORMANCE + TIMELINE
IMPORTANT SPEECH INSTRUCTIONS
EXACT SPOKEN PERSIAN
PRONUNCIATION REQUIREMENTS
FACIAL / BODY PERFORMANCE
AUDIO
VISUAL STYLE
STRICT NEGATIVE CONSTRAINTS
FINAL SUCCESS TEST
```

### Speech contract

- هر phrase زمان خودش را دارد.
- pause واقعی تعریف می‌شود.
- در pause:
  - no speech
  - no whisper
  - no filler sound
  - mouth closed
  - no mouthing next sentence
- high energy به معنی fast speech نیست.
- قدرت Hook از eye contact + facial expression + stronger voice می‌آید، نه عجله.

---

# 4) Persian pronunciation — یادگیری کلیدی

اعراب‌گذاری فقط برای واژه‌های پرریسک، نه کل متن.

نمونه واژه‌های حساس:

- `جِمِنای`
- `فِلو`
- `تِلِگرام`
- `یِک‌دَقیقه‌ای`

### Rule مهم

اگر یک ترکیب خراب تلفظ می‌شود، اول syntax جمله را ساده کن.

نمونه:

- `می‌سازتش` → `خودش برات می‌سازه.`
- CTA مشکل‌دار با punctuation زیاد → یک phrase پیوسته.

---

# 5) Duck.ai — آخرین baseline قفل‌شده

## Hook production-safe

`پول اشتراک نده. حتی ثبت نام هم نکن!`

## ادامه

`چندتا هوش مصنوعی معروف رو رایگان یه جا داری`

`عکس هم می‌سازه.`

## CTA

`اگه میخوایش: همه رو کامنت کن.`

### Learning

- keyword را isolate نکن اگر مدل روی آن restart می‌کند.
- punctuation قبل از keyword می‌تواند segmentation مصنوعی بسازد.
- exact dialogue باید قبل از prompt lock شود.
- اسم ابزار داخل spoken Reel لازم نیست؛ reveal در cover/caption/comment reply انجام می‌شود.

---

# 6) Z.ai — baseline موفق

Hook:

`پول نده، سایتتو رایگان بساز!`

Dialogue structure:

- Hook
- real silence
- `فقط بگو چه سایتی میخوای، خودش برات می‌سازه.`
- real silence
- `بدون کدنویسی.`
- real silence
- CTA

### Cover learning

هرچه طراحی خلوت‌تر شد، Hook بهتر دیده شد.

Direction نهایی:

- white + blue
- website-builder atmosphere
- character مناسب و طبیعی
- logo
- URL `chat.z.ai`
- فقط headline اصلی و عناصر ضروری

---

# 7) Detective / Gemini Live — visual system موفق

برای hookهایی مثل:

- `گوشیتو می‌گرده؟`
- `صفحه گوشیتو می‌بینه.`
- `حتی می‌فهمه چه برنامه‌ای باز کردی.`

سبک generic جواب ضعیف‌تری داشت؛ style معمایی/پلیسی بهتر بود:

- dark navy / black
- purple/magenta neon
- electric blue
- clue/search/mystery feeling
- subtitle cardهای جدا و cinematic

### Strength

طراحی فقط «زیبا» نبود؛ mood محتوای Reel را منتقل می‌کرد.

---

# 8) Cover design — چیزی که user بیشتر تأیید کرد

- headline خیلی بزرگ
- 1 payoff رنگی
- composition موبایل‌محور
- typography فارسی سه‌بعدی یا bold، ولی readable
- subject/character واضح
- clutter کم
- عناصر کمکی فقط وقتی story را تقویت می‌کنند

### Safe Zone

- 1080×1920
- بالا 210–270px
- پایین حداقل 310–350px؛ در صورت نیاز تا 450px
- چپ حداقل 60px
- راست 84–120px
- محتوا تا حد ممکن در مرکز برای Grid crop

### Golden rule

اگر audience در یک ثانیه تیتر را نمی‌خواند، decoration باید کم شود.

---

# 9) Subtitle PNG — baseline جدید

User چند بار تأکید کرد که subtitleها باید:

- جدا جدا باشند.
- PNG transparent باشند.
- فارسی دقیق داشته باشند.
- paragraphها طبق درخواست وسط‌چین باشند.
- با رنگ و فضای خود Reel هماهنگ باشند.
- generic نباشند.
- برای placement روی ویدیو compact باشند.

### بهترین نتیجه

وقتی cardها:

- 1 یا 2 رنگ اصلی داشتند.
- 1 keyword برجسته می‌شد.
- icon کوچک مرتبط داشتند.
- canvas tight بود.
- متن ساده و readable باقی می‌ماند.

---

# 10) RTL و فارسی — خط قرمز

مشکل‌هایی که باید از این به بعد zero-tolerance باشند:

- حرف یا کلمه اشتباه
- جاافتادگی
- جابه‌جایی RTL
- paraphrase ناخواسته
- English داخل جمله فارسی که layout را برعکس می‌کند
- punctuation خراب

### Quality Gate

هر asset قبل از تحویل باید copy user را **کلمه‌به‌کلمه** پاس کند.

Design زیبا با متن غلط = خروجی ردشده.

---

# 11) Visual language بر اساس موضوع

| موضوع | Visual direction |
|---|---|
| AI tools / general tech | dark charcoal + high contrast accent |
| Duck.ai | black + yellow + white / optional teal accent |
| Z.ai website | white + blue, clean tech |
| Gemini Live mystery | navy + purple + magenta + electric blue |
| Skincare | ivory + champagne gold + warm brown |
| Clay child | peach + cream + soft pink 3D |
| Tehran future | navy + cyan + violet futuristic |
| Money/free hook | red/black یا yellow/black فقط اگر داستان مالی است |

---

# 12) Character consistency

## Rose

Rose زمانی که character-led Reel داریم باید فوراً قابل‌شناسایی بماند:

- Persian woman ~25
- oval youthful face
- thin round black glasses
- chin-length bob
- dark roots
- hot-magenta front/outer sections
- sapphire/electric-blue underlayer

لباس می‌تواند تغییر کند؛ identity نه.

## Other characters

اگر Reel character دیگری دارد، همان image/video واقعی باید source reference باشد و character نباید بی‌دلیل با Rose جایگزین شود.

---

# 13) Website Discover — cross-channel insight

برای کارت‌های Discover سایت، بهترین کار این است که از Cover همان Reel یا adaptation بسیار نزدیک استفاده شود.

چرا؟

کاربر از Instagram وارد سایت می‌شود و باید همان Reel را فوری تشخیص دهد.

### Rule

Instagram cover → website Discover visual continuity.

نه یک artwork کاملاً متفاوت که recognition را از بین ببرد.

---

# 14) Telegram assets

Telegram image باید:

- visual language Reel را حفظ کند.
- headline واضح داشته باشد.
- برای آموزش/لینک/برنامه فضای کافی داشته باشد.
- CTA و username واضح ولی ثانویه باشند.

اگر Telegram مقصد کامل آموزش است، Reel نباید تمام method را از قبل لو دهد.

---

# 15) Strengthهای کار ما در این چرخه

## 1. سرعت تبدیل feedback به rule

Feedbackهایی مثل:

- «ماشینی می‌گه»
- «خیلی شلوغه»
- «فارسی اشتباهه»
- «سبک پلیسی باشه»
- «وسط‌چین کن»

به ruleهای قابل‌تکرار تبدیل شدند.

## 2. Visual adaptability

برای هر Reel یک style واحد به همه‌چیز تحمیل نکردیم؛ genre-specific direction ساختیم.

## 3. Hook-first thinking

Cover، subtitle و script همگی Hook را در اولویت قرار دادند.

## 4. Strong continuity

Character، palette، cover و Discover image می‌توانند یک funnel بصری واحد بسازند.

## 5. Exact-production mindset

از «یک prompt زیبا» به سمت:

`script lock → prompt lock → render QA → visual pack → publish funnel`

رفتیم.

---

# 16) Failureهایی که نباید تکرار شوند

- تولید asset برای متن/موضوع قبلی به‌جای درخواست فعلی.
- ادامه‌دادن از context اشتباه وقتی user copy جدید داده.
- subtitle غیرمجزا وقتی user جداگانه خواسته.
- Persian text wrong یا ناقص.
- طراحی generic بدون توجه به ویدیو.
- over-effects و glow زیاد.
- cover شلوغ.
- reveal کردن tool name وقتی curiosity باید حفظ شود.
- تغییر بی‌دلیل character.
- ارائه چند variant وقتی user یک خروجی دقیق می‌خواهد.

### Anti-confusion rule

**آخرین user message همیشه task active است.**

قبل از تولید هر asset:

1. exact requested text را extract کن.
2. count deliverables را مشخص کن.
3. style reference آخر را مشخص کن.
4. current Reel/video را مشخص کن.
5. هیچ متن یا موضوع قدیمی را وارد output نکن مگر user صریحاً خواسته باشد.

---

# 17) Default checklist برای Reel بعدی

- [ ] Topic و goal روشن است.
- [ ] exact dialogue lock شده.
- [ ] یک CTA داریم.
- [ ] اگر Flow است، speech blocks کوتاه‌اند.
- [ ] silence واقعی داریم.
- [ ] pronunciation-risk words مشخص‌اند.
- [ ] character/reference mode درست است.
- [ ] tool reveal strategy مشخص است.
- [ ] video واقعی QA شده.
- [ ] cover Hook-first است.
- [ ] safe zone رعایت شده.
- [ ] subtitleها جدا و transparent هستند.
- [ ] Persian exactness pass شده.
- [ ] visual palette با Reel match است.
- [ ] Telegram/Discover continuity در صورت نیاز حفظ شده.

---

# 18) Source of Truth

برای Reelهای بعدی این فایل‌ها با هم خوانده شوند:

- `06_workflows/reels-flow-production-playbook.md`
- `07_templates/reel-end-to-end-chat-starter-template.md`
- `10_feedback-learning/feedback-ledger.md`
- `10_feedback-learning/reels-learning-log-2026-09-03.md`
- `10_feedback-learning/reels-ai-tools-cycle-2026-09-03.md`
- `11_prompt-libraries/flow-reels-approved-prompts.md`
- `11_prompt-libraries/flow-reels-approved-ai-tools-2026-09-03.md`
- `12_design/reels-cover-subtitle-style-guide.md`

قاعده نهایی: **از baseline تأییدشده شروع کن، نه از صفر.**
