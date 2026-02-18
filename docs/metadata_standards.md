# METADATA AND DATA STANDARDS
## VERSION 1.0 | IYEDEX DATA INITIATIVE

To ensure that the data collected is usable for training 3amAli, **all submissions must adhere to the Script Separation Standard**.

> **💡 بالتونسي:**
> هذا "الكود" ولا "الهيكلة" اللي لازم نتبعوه باش 3amAli يفهمنا بالقدا. لازمنا نكونو منظمين باش الداتا تكون نظيفة.

---

## CORE FORMAT: JSONL
*(بنية الملفات)*

We use **JSON Lines (JSONL)** format. This means every line in the file is a valid, independent JSON object. Do not wrap the file in a list `[...]`.

> **💡 يعني:**
> كل سطر هو معلومة كاملة. ما تحطش فاصلة (comma) في آخر السطر، وما تحطش أقواس مربعة (brackets) في أول وآخر الملف.

### The Standard Object
*(الكائن القياسي)*

Every object must have a Question (`q`) and an Answer (`a`).

```json
{"q": "Your question here", "a": "Your answer here"}
```

---

## SCRIPT SEPARATION RULES
*(قواعد الكتابة)*

We do not mix scripts in the same file. You must choose the correct folder based on the script you are writing in.

> **💡 بالتونسي:**
> ما تخلطش الفرونكو مع العربي. كل واحد في دوسي وحدو.

### 1. Tunisian Arabic Script (Folder: `tunisian`)
*(اللغة العربية التونسية)*

*   **Path**: `data/text/q_a/tunisian/`
*   **Rule**: Use Arabic script only. Write natural, spoken Tunisian.
*   **Valid Example**: `{"q": "وينك؟", "a": "لباس الحمد لله"}`

> **💡 بالتونسي:**
> استعمل الحروف العربية أكهو. اكتب كيما تتكلم مع صاحبك، أما بالحروف العربية.

### 2. Franco / Tunizi (Folder: `franco`)
*(الفرونكو / تونيزي)*

*   **Path**: `data/text/q_a/franco/`
*   **Rule**: Use Latin script with numbers for specific sounds.
*   **Mapping**:
    - `3` = ع (3in)
    - `7` = ح (7a)
    - `9` = ق (9af)
    - `5` = خ (5a)
    - `2` = ء (Hamza)
*   **Valid Example**: `{"q": "wink?", "a": "labes hamdoullah"}`

> **💡 بالتونسي:**
> استعمل الحروف اللاتينية والأرقام المعروفة في تونس (كيما 3 و 7 و 9).

---

## FILE NAMING
*(اسم الملف)*

*   Use **snake_case** for files and folders (e.g., `my_new_file.jsonl`).
*   Do not use spaces or CamelCase.
*   Extension must be **.jsonl**.

> **💡 يعني:**
> ما تعملش espace في اسم الفايل. استعمل "underscore" (_) في بلاصة l'espace. وديمة minuscule (صغير).
>
> *   `ghneya_jdida.jsonl` ✅
> *   `Ghneya Jdida.json` ❌
