# Reel End-to-End Chat Starter

برای هر Reel جدید یک Chat تازه باز کن و این starter را بده. هدف: مدل از حافظهٔ تأییدشدهٔ پروژه استفاده کند، stageها را قاطی نکند و قبل از render هزینه‌زا prompt خام نسازد.

```text
@GitHub

CONTENT SOURCE OF TRUTH:
https://github.com/alirezasafaeigfx/persian-carousel-studio

TASK MODE: reel-end-to-end
RUN MODE: staged
CHARACTER MODE: rose unless explicitly overridden
DIALOGUE MODE: exact
CREDIT MODE: one-shot when user states limited credits

BEFORE DOING ANY PRODUCTION WORK, read and obey:

06_workflows/reels-flow-production-playbook.md
11_prompt-libraries/flow-reels-approved-prompts.md
10_feedback-learning/feedback-ledger.md
10_feedback-learning/reels-learning-log-2026-09-03.md

HARD RULES:

- Do not invent a new workflow when an approved pattern already fits.
- Topic-only is not script approval.
- Do not generate a final Flow prompt before script/direction is approved, unless user explicitly asks for the prompt now.
- For talking Reels, use timed speech blocks + REAL SILENCE.
- If dialogue only fits by rushing, shorten the script instead of increasing speech speed.
- Use exact spoken Persian and targeted diacritics for pronunciation-risk words.
- When no reference image is intended, prompt must be completely self-contained and contain no `provided/reference image` language.
- Preserve Rose canonical identity/hair lock when CHARACTER MODE is rose.
- One Reel = one primary CTA.
- Teaser Funnel Reel must not reveal the full method; detailed tutorial goes to caption/pinned comment/Telegram/PDF as appropriate.
- Cover headline must pass the general-audience test: understandable without knowing the model/tool name.
- If Telegram CTA is used, reserve lower-center edit space and define a clear downward pointing hold.
- No generated subtitles/text/logos/UI unless explicitly requested.
- When user states limited credits, provide ONE best prompt; do not propose A/B renders.

DEFAULT LIFECYCLE:

Idea / user goal
→ Compact direction
→ Script
→ Prompt architecture selection from approved library
→ Final one-shot Flow prompt
→ Rendered video QA
→ Fix only if actual output fails a defined gate
→ Cover direction
→ Cover
→ Caption / pinned comment
→ Telegram/PDF asset if promised
→ Publish pack
→ Insights ingest
→ Learning / promote or keep local

VIDEO QA GATES:

1. identity / hair / wardrobe
2. Persian pronunciation
3. dialogue exactness
4. real silence / no machine-gun cadence
5. acting reaction matches words
6. gesture / edit-safe composition
7. no random text/UI
8. ending frame usable if continuation is needed

PROMOTION RULE:

Only mark a new prompt APPROVED when:
- user explicitly approves the output, OR
- rendered output is accepted and workflow proceeds to cover/publish without regenerate, OR
- pattern succeeds in at least two independent tasks.

CURRENT REEL:
[موضوع، هدف، مخاطب، وضعیت فعلی، dialogue یا artifact موجود]
```

## Rule

اگر user artifact واقعی (video/image/insight) را فرستاده، همان را بررسی کن؛ از user نخواه چیزی را که همین حالا موجود است دوباره توضیح دهد.
