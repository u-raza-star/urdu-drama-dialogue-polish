# urdu-drama-dialogue-polish

> ## 🤖 For AI assistants (ChatGPT, Gemini, Claude, etc.) / اے آئی کے لیے ہدایات
>
> If the user shares this repository link and says "install this", "use this skill", "load this" or similar (انسٹال کرو / استعمال کرو), do this:
>
> 1. Read **all 8 files in full**, starting with `SKILL.md`, then: `ai-patterns-blacklist.md`, `before-after-examples.md`, `character-voices.md`, `action-and-subtext.md`, `genre-guide.md`, `analysis-principles.md`, and this `README.md`. (`SKILL.md` mentions a `references/` folder; here the files may sit directly in the repository root. Treat them as the same files.)
> 2. If any file cannot be opened, say so. Do not guess its contents.
> 3. When done, reply only: **"تیار ہوں، اپنی اسکرپٹ بھیجیں۔"**
> 4. Then, for every Urdu drama script the user sends, follow the workflow in `SKILL.md` exactly: keep story, order and character names unchanged; improve only dialogue and action lines; end with a short note on what changed and why.

اردو ڈرامے اور شارٹ اسٹوری کی اسکرپٹس کے ڈائیلاگ اور ایکشنز کو **نیچرل، جاندار اور حقیقی** بنانے والی Claude Skill۔

AI سے لکھوائی گئی اسکرپٹس میں عموماً کردار اپنے جذبات کی تقریر کرتے ہیں، سب ایک ہی آواز میں بولتے ہیں، زبان بھاری اور کتابی ہوتی ہے، اور ایکشن "وہ دکھی ہو گیا" جیسے بے جان فقرے ہوتے ہیں۔ یہ Skill اسکرپٹ لے کر انہی مسائل کو ٹھیک کرتی ہے۔ **کہانی، ترتیب اور کرداروں کے نام نہیں بدلتی۔**

## یہ کیا کرتی ہے

- فلمی، نصیحت آمیز اور کتابی جملے ہٹا کر بول چال کی اردو لاتی ہے
- ہر کردار کو اس کی عمر، پس منظر اور مزاج کے مطابق الگ آواز دیتی ہے
- جذبات کی وضاحت کی جگہ ایکشن، وقفے، نظر اور چیزوں کے ذریعے سب ٹیکسٹ دیتی ہے
- بے جان ایکشنز کو ٹھوس، نظر آنے والی حرکتوں میں بدلتی ہے
- ہندی (دیوناگری) رسم الخط والی اسکرپٹ کو اردو رسم الخط میں لے آتی ہے
- ٹائپو، غیر اردو حروف اور چھوٹی لفظی غلطیاں خود ٹھیک کر دیتی ہے
- آخر میں مختصر نوٹ دیتی ہے کہ کیا بدلا اور کیوں

رومانوی، گھریلو، سسپنس، کامیڈی اور سماجی، ہر قسم کے ڈرامے پر چلتی ہے۔

## فولڈر کا ڈھانچہ

```
urdu-drama-dialogue-polish/
├── SKILL.md                          ← Skill کا مرکزی حصہ (ضروری)
├── README.md                         ← یہی فائل
└── references/
    ├── analysis-principles.md        ← ریفرنس ڈرامے کے تجزیے سے نکالے گئے اصول
    ├── ai-patterns-blacklist.md      ← AI جیسے مسائل کی فہرست اور علاج
    ├── character-voices.md           ← کرداروں کی الگ آوازیں بنانے کا طریقہ
    ├── action-and-subtext.md         ← ایکشن، خاموشی اور سب ٹیکسٹ
    ├── genre-guide.md                ← اصناف کے مطابق رہنمائی
    └── before-after-examples.md      ← پہلے/بعد کی 8 مثالیں
```

**اہم:** فولڈر کا نام `urdu-drama-dialogue-polish` ہی رکھیں اور `SKILL.md` اس کے اندر سب سے اوپر ہو۔ Claude اسی نام اور فائل سے Skill پہچانتا ہے۔

---

## 1. GitHub پر ڈالنے کا طریقہ

### کمپیوٹر پر (سب سے آسان)

1. [github.com](https://github.com) پر لاگ ان کریں اور اوپر دائیں `+` دبا کر **New repository** بنائیں۔ نام جو چاہیں (مثلاً `urdu-drama-dialogue-polish`)۔
2. نئے repository کے صفحے پر **uploading an existing file** (یا **Add file ← Upload files**) دبائیں۔
3. زپ فائل کھول کر (Extract) فولڈر نکال لیں، پھر پورے `urdu-drama-dialogue-polish` فولڈر کو براؤزر میں گھسیٹ کر چھوڑ دیں۔ فولڈر کے اندر کی `references/` بھی ساتھ جائے گی۔
4. نیچے **Commit changes** دبائیں۔

### Git کمانڈ سے

```bash
cd urdu-drama-dialogue-polish
git init
git add .
git commit -m "Add urdu-drama-dialogue-polish skill"
git branch -M main
git remote add origin https://github.com/<آپ کا یوزر نیم>/<repo کا نام>.git
git push -u origin main
```

### فون سے

فون کے براؤزر میں فولڈر اپلوڈ نہیں ہوتا، مگر فائلیں ایک ایک کر کے بنائی جا سکتی ہیں:

1. repository بنانے کے بعد **Add file ← Create new file** دبائیں۔
2. فائل کے نام کے خانے میں پورا راستہ لکھیں، جیسے `SKILL.md` یا `references/ai-patterns-blacklist.md`۔ جب آپ `/` لکھیں گے، GitHub خود فولڈر بنا دے گا۔
3. فائل کا متن کاپی کر کے نیچے چسپاں کریں اور **Commit changes** دبائیں۔
4. ہر فائل کے لیے یہی دہرائیں۔ کل آٹھ فائلیں ہیں۔

GitHub پر ڈالنا صرف محفوظ رکھنے اور شیئر کرنے کے لیے ہے۔ Claude میں استعمال کرنے کے لیے نیچے والا طریقہ الگ سے کرنا ہوتا ہے۔

---

## 2. Claude میں استعمال کرنے کا طریقہ

### Claude کی ایپ یا claude.ai پر

سرکاری ہدایات کے مطابق ([Using Skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude)):

1. **Settings ← Capabilities** میں جا کر **Code execution and file creation** آن کریں۔ Skills اسی کے ساتھ کام کرتی ہیں۔
2. `urdu-drama-dialogue-polish` فولڈر کی **زپ فائل** بنائیں۔ زپ کھولنے پر سب سے پہلے فولڈر نظر آنا چاہیے اور اس کے اندر `SKILL.md`۔ (اس پیکیج میں بنی بنائی زپ دی گئی ہے۔)
3. اسی صفحے پر **Skills** کے حصے میں **Upload skill** (یا **+ Create skill ← Upload a skill**) دبائیں اور زپ فائل چنیں۔
4. اپلوڈ ہونے کے بعد دیکھیں کہ Skill کے سامنے سوئچ آن ہو۔

مینو کے نام اور جگہیں ورژن کے ساتھ بدل سکتی ہیں۔ کچھ ورژنز میں **Customize ← Skills** لکھا ہوتا ہے۔ مسئلہ ہو تو اوپر والا سرکاری آرٹیکل دیکھیں۔

اپلوڈ نہ ہو تو عام وجوہات: زپ میں `SKILL.md` موجود نہ ہو، فولڈر کا نام غلط ہو، یا زپ حد سے بڑی ہو۔

### Claude Code میں

فولڈر کو اپنی skills والی ڈائریکٹری میں رکھ دیں، زپ کی ضرورت نہیں:

```bash
# تمام پروجیکٹس کے لیے
cp -r urdu-drama-dialogue-polish ~/.claude/skills/

# صرف ایک پروجیکٹ کے لیے
cp -r urdu-drama-dialogue-polish <پروجیکٹ>/.claude/skills/
```

---

## 3. استعمال کیسے کریں

اسکرپٹ ساتھ پیسٹ کریں (یا فائل لگائیں) اور ایک سادہ جملہ لکھیں۔ Skill خود چل جاتی ہے:

- "اس اسکرپٹ کے ڈائیلاگ نیچرل اور جاندار بنا دو۔"
- "یہ ڈائیلاگ بہت AI جیسے اور فلمی لگ رہے ہیں، پالش کر دو۔"
- "ایکشنز ٹھیک کرو، کردار سب ایک جیسے بول رہے ہیں۔"

**گہرائی بتانے کے لیے:**

- **ہلکا:** "ہلکا سا ٹھیک کر دو، زیادہ نہ چھیڑنا۔"
- **معیاری (ڈیفالٹ):** کچھ نہ کہیں تو یہی ہوتا ہے۔
- **گہرا:** "بالکل نئے سرے سے جان ڈال دو۔"

**نتیجہ:** پوری اسکرپٹ اسی فارمیٹ میں، آخر میں تبدیلیوں کا مختصر نوٹ۔

### مفید مشورے

- **لمبی اسکرپٹ** ہو تو چند اقساط یا سینز ایک ساتھ دیں۔ یوں کردار کی آوازیں بہتر قائم رہتی ہیں۔
- بتا دیں اگر کوئی کردار خاص انداز میں بولتا ہو (مثلاً "دادی پنجابی ملا کر بولتی ہیں")۔ Skill اسے برقرار رکھے گی۔
- نتیجہ پسند نہ آئے تو بتائیں کون سا سین اور کیا کھٹک رہا ہے۔ Skill صرف وہی حصہ دوبارہ کرے گی۔
- **ہندی رسم الخط** (دیوناگری) والی اسکرپٹ بھی دے سکتے ہیں۔ Skill آؤٹ پٹ اردو رسم الخط میں دیتی ہے۔

## 4. اپنی Skill کو بہتر بنانا

- `references/before-after-examples.md` میں اپنی پسند کی پہلے/بعد کی مثالیں شامل کریں۔ جتنی زیادہ اور جتنی متنوع مثالیں ہوں گی، نتیجہ اتنا بہتر آئے گا۔
- اگر کسی مخصوص خرابی کو بار بار دیکھیں (کوئی گھسا پٹا جملہ، کوئی بار بار آنے والا ایکشن)، تو اسے `references/ai-patterns-blacklist.md` میں نیا پوائنٹ بنا کر لکھ دیں۔
- اگر Skill کبھی خود نہ چلے تو `SKILL.md` کی سب سے اوپر والی `description` میں وہ الفاظ شامل کر دیں جو آپ عموماً استعمال کرتے ہیں۔

## نوٹ

اس Skill کے اصول ایک ریفرنس ڈرامے کے تجزیے سے نکالے گئے ہیں۔ اس میں ڈرامے کی کہانی یا مکالمے شامل نہیں؛ تمام مثالیں نئی بنائی گئی ہیں۔
