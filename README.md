# 🇹🇳 TUNISIAN DATA HUB

## THE OPEN NATIONAL DATASET FOR ARTIFICIAL INTELLIGENCE
*(El Maktba el Wataniya el Maftou7a 3la El "AI" wil Data)*

Tunisian Data Hub is a massive, high-granularity digital library created and licensed by **IyedeX**. This repository is the foundational training ground for **3amAli** and any future Tunisian AI models. It is designed to be the "Wikipedia of Tunisian Data"—open for the community to enrich, refine, and expand.

> **💡 Bil Tounsi:**
> Hatha projet kbir bach najmou na3mlou "Intelligence Artificielle" Tounsiya 100%. Hatha el "base" mta3 3amAli. Ay wa7ed fina inajjem i3awen, hatta b'kelma wala b'nokat wala b'recette mta3 makla. Hatha kima "Wikipedia" mta3na a7na.

---

## PROJECT CORE ARCHITECTURE
*(Kifach M9assma el 5edma?)*

The structure is optimized for **Large Language Models (LLMs)**. We use a simplified 4-folder base structure where you can organize your data flexibly, but every entry must be trilingual (Tunisian, Franco, English) to ensure maximum utility for AI training.

> **💡 Sahla Barcha:**
> 9assmna el data l'4 dossiyet kbar. Kol dossi fih naw3 mta3 ma3loumat. Enti tnajjem tziid ay fichier json t7eb 3lih dakhil ay dossi menhom.

| BASE FOLDER   | FOCUS                 | OBJECTIVE (Chnwa n7ottou fih?)                                                          |
| ------------- | --------------------- | --------------------------------------------------------------------------------------- |
| **CHATS**     | `data/text/chats`     | **Klem w 7adith**: Conversations, Q&A, and dialogues. (Ay 7keya fiha sou2al w jwab)     |
| **DICTONARY** | `data/text/dictonary` | **Klem w Ma3neuh**: Definitions, slang explanations. (Kima el mounjed, ama b'eddarja)   |
| **KNOWLEDGE** | `data/text/knowledge` | **Thaqafa w Tarikh**: General knowledge, history, facts, jokes. (Tarikh, Nokat, Amthal) |
| **LIFESTYLE** | `data/text/lifestyle` | **Hyet w Jaw**: Music, food, daily life. (Makla, Ghna, Koura, Mosalslet)                |

---

## FILE STRUCTURE
*(Win n7ot el Fichier mte3i?)*

This structure is designed for "Ease of Entry." You can create **any JSON file or sub-folder** you want inside the 4 base directories.

> **💡 7orr fi khtiyarak:**
> Mate7sebhech barcha. A3mel fichier jdid, sammih esm wadha7, w 7ottou fil dossi elli tchoufou a9reb.

```text
tunisian-data/
├── data/
│   └── text/
│       ├── chats/           | e.g. 7adith_fil_marchi.json, sbe7_el_khir.json
│       ├── dictonary/       | e.g. klem_sfaxi.json, klem_za3ama.json
│       ├── knowledge/       | e.g. dates_historiques.json, amthal_cha3biya.json
│       └── lifestyle/       | e.g. recette_couscous.json, ghne_rap_tounsi.json
└── docs/
    ├── metadata_standards.md
    └── contribution_guide.md
```

**Rule:** You can organize sub-folders however you like (e.g., `knowledge/history/roman_era/`), as long as they stay within the meaning of the 4 base categories.

---

## DATA FORMATS
*(Kifach Nektbou el Data?)*

To make this dataset ready for training (GPT, Llama, 3amAli), **EVERY** entry must follow this trilingual format. This allows the AI to understand the script, the phonetics, and the meaning.

> **💡 Aham 9a3da:**
> Lazem dima tektel el joumla b'3loughat: Tounsi (Arabe), Tounsi (Latin/Franco), w Anglais (Ma3neha).

### Universal Format
*(Exemple S7i7)*

**File: `data/text/any_folder/your_file.json`**

```json
[
  {
    "tunisian": "شنوة الجو؟",
    "franco": "chnowa el jaw?",
    "english": "How is it going? / What's up?"
  },
  {
    "tunisian": "لاباس، الحمد لله.",
    "franco": "labes, hamdoullah.",
    "english": "Good, thanks to God."
  }
]
```

---

## HOW TO CONTRIBUTE (EASY STEPS)
*(Kifach T3awenna?)*

You don't need to be an AI expert to help. Just follow these steps:

1. **FORK**: Click the 'Fork' button at the top of this repo. *(A3mel Copie 3andek)*
2. **PICK A BASE FOLDER**: Choose one of the 4 bases: `chats`, `dictonary`, `knowledge`, `lifestyle`. *(Ekhtar dossi)*
3. **ADD DATA**: Create a new `.json` file or a new folder. *(Zid fichier jdid)*
4. **FORMAT**: **CRITICAL**: You must include `tunisian`, `franco`, and `english` for every piece of text. *(Ekteb b'3 loughat)*
5. **PULL REQUEST**: Submit your changes for review. *(Ab3ath el 5edma)*

---

## GOVERNANCE & LICENCE

* **Created By**: **IyedeX**
* **Purpose**: Training **3amAli** and empowering the Tunisian AI ecosystem.
* **Licence**: **Creative Commons Attribution 4.0 International (CC BY 4.0)**.
* *You are free to share and adapt the data, but you must give credit to IyedeX and the community contributors.*

---

## COMMUNITY SUPPORT

For complex data structures or big data dumps, please open an **Issue** or contact the **IyedeX** team directly. Let's build the largest open brain for Tunisia.
