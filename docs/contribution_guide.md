# CONTRIBUTION GUIDE

## HELP BUILD TUNISIAN AI WITH IYEDEX
*(آيا معانا باش نبنيو ذكاء اصطناعي تونسي)*

Thank you for contributing to the **Tunisian Data Hub**! This project is the collective brain of the Tunisian AI ecosystem. By contributing, you are helping **3amAli** understand our dialect, our culture, and our reality.

> **💡 بالتونسي:**
> يعطيك الصحة! كي تزيد حاجة هوني، راك قاعد تعلم في "عم علي" كيفاش يتكلم و يفهم كيما التوانسة. كل كلمة، كل نكتة، كل مثل عندو قيمة كبيرة.

---

## STEP-BY-STEP SUBMISSION
*(خطوات المساهمة)*

### STEP 1: FORK & CLONE
*(اعمل نسخة)*

1. Click **Fork** (top right button). *(الفوق على اليمين)*
2. Clone to your PC:
   `git clone https://github.com/iyedex-labs/tunisian-data` *(انسخ الرابط هذا)*

### STEP 2: CHOOSE YOUR CATEGORY
*(وين تحط الخدمة؟)*

Go to `data/text/` and pick the right folder. Most contributions will go to `q_a`.

| Category       | Folder                 | Content                            |
| :------------- | :--------------------- | :--------------------------------- |
| **Q&A**        | `data/text/q_a`        | Questions and Answers (سؤال وجواب) |
| **Dictionary** | `data/text/dictionary` | Definitions (شرح كلمات)            |
| **Knowledge**  | `data/text/knowledge`  | Facts and History (ثقافة وتاريخ)   |
| **Lifestyle**  | `data/text/lifestyle`  | Food, Music, etc. (ماكلة، جو، فن)  |

### STEP 3: CHOOSE YOUR SCRIPT
*(اختار نوع الكتيبه)*

**CRITICAL RULE**: Do not mix scripts.
*   If you are writing in **Arabic Script**, go to the `tunisian` folder. **(عسلامة شحالك)**
*   If you are writing in **Latin/Franco**, go to the `franco` folder. **(3slama ch7alek)**

> **💡 مهم برشا:**
> ما تخلطش الفرونكو مع العربي. كل واحد في دوسي وحدو.

### STEP 4: ADD DATA (JSONL Format)
*(زيد الداتا)*

Create a new file with extension `.jsonl` (e.g., `football_talk.jsonl`).
Each line must be a separate JSON object:

```json
{"q": "question here", "a": "answer here"}
```

### STEP 5: COMMIT AND PUSH
*(سجل و ابعث)*

1. `git add .`
2. `git commit -m "added new football Q&A"`
3. `git push origin dev`

### STEP 6: OPEN A PULL REQUEST
*(ابعث الخدمة لينا)*

Go to GitHub and open a "Pull Request". We will review it and merge it! 

*(متنساش تعمل "pull request" باش الخدمة توصل لينا)*
