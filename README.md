# 🇹🇳 TUNISIAN DATA HUB

## THE OPEN NATIONAL DATASET FOR ARTIFICIAL INTELLIGENCE
*(المكتبة الوطنية المفتوحة للذكاء الاصطناعي والبيانات)*

Tunisian Data Hub is a massive, high-granularity digital library created and licensed by **IyedeX**. This repository is the foundational training ground for **3amAli** and any future Tunisian AI models. It is designed to be the "Wikipedia of Tunisian Data"—open for the community to enrich, refine, and expand.

> **💡 بالتونسي:**
> هذا مشروع كبير باش ننجّموا نعملوا "ذكاء اصطناعي" تونسي 100%. هذه هي القاعدة متاع "عم علي". أي واحد فينا ينجم يعاون، حتى بكلمة ولا بنكتة ولا بوصفة متع ماكلة. هذي كيما "ويكيبيديا" متاعنا أحنا.

---

## PROJECT CORE ARCHITECTURE
*(كيفاش مقسمة الخدمة؟)*

The structure is optimized for **Large Language Models (LLMs)**. We use a folder-based structure where data is separated by **Script Type** (Tunisian Arabic Script vs. Franco/Latin Script).

> **💡 ساهلة برشا:**
> قسمنا الداتا لملفات حسب النوع (كيما الأسئلة والأجوبة `q_a`)، وفي وسط كل نوع, نقسموهم حسب الكتيبه: يا اما بالعربي (tunisian) يا اما بالاحرف اللاتينية (franco).

### Directory Structure
*(هيكلة الملفات)*

```text
tunisian-data/
├── data/
│   └── text/
│       ├── q_a/                 | Question & Answer Datasets (سؤال وجواب)
│       │   ├── franco/          | Files written in Latin script + numbers (فرونكو)
│       │   │   └── education.jsonl
│       │   └── tunisian/        | Files written in Arabic script (تونسي بالعربي)
│       │       └── general.jsonl
│       ├── dictionary/          | (قاموس)
│       ├── knowledge/           | (ثقافة عامة)
│       └── lifestyle/           | (نمط عيش)
└── docs/
    ├── metadata_standards.md
    └── contribution_guide.md
```

---

## DATA FORMATS
*(كيفاش نكتبوا الداتا؟)*

We use **JSONL (JSON Lines)** format. Each line is a separate JSON object containing a question `q` and an answer `a`.

> **💡 اهم قاعدة:**
> كل سطر داتا لازمو يكون فيه "سؤال" و "جواب". ما نخلطوش العربي مع الفرونكو في نفس الملف.

### 1. Franco (Tunizi)
**Path:** `data/text/q_a/franco/*.jsonl`
*(مثال بالفرونكو)*

```json
{"q": "chnowa a7sen fac informatique?", "a": "insat w esprit behin barcha, chouf zeda isi."}
{"q": "kifeh nriviz l bac?", "a": "a3mel planning w rkz 3al matiere principale."}
```

### 2. Tunisian (Arabic Script)
**Path:** `data/text/q_a/tunisian/*.jsonl`
*(مثال بالعربي)*

```json
{"q": "شنوا رايك فيه؟", "a": "والله حاجة باهية برشا، ننصح بيها."}
{"q": "كيفاش نخدم الويفي؟", "a": "انزل عالزر اللي فيه الاشارة واستنى شوية تو يخدم."}
```

---

## HOW TO CONTRIBUTE
*(كيفاش تعاوننا؟)*

1. **FORK**: Click the 'Fork' button at the top of this repo. *(اعمل نسخة عندك)*
2. **CHOOSE A CATEGORY**: Navigate to `data/text/` and pick a category (e.g., `q_a`). *(اختار دوسي)*
3. **CHOOSE A SCRIPT**: Go into `tunisian` (for Arabic script) or `franco` (for Latin script). *(اختار الكتيبه)*
4. **ADD DATA**: Create a new `.jsonl` file. *(زيد ملف جديد)*
5. **PULL REQUEST**: Submit your changes. *(ابعث الخدمة)*

---

## GOVERNANCE & LICENSE

* **Created By**: **IyedeX**
* **Purpose**: Training **3amAli** and empowering the Tunisian AI ecosystem.
* **License**: **Creative Commons Attribution 4.0 International (CC BY 4.0)**.
* *You are free to share and adapt the data, but you must give credit to IyedeX and the community contributors.*

---

## COMMUNITY SUPPORT

For complex data structures or big data dumps, please open an **Issue** or contact the **IyedeX** team directly. Let's build the largest open brain for Tunisia.
