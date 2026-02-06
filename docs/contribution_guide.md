# CONTRIBUTION GUIDE

## HELP BUILD TUNISIAN AI WITH IYEDEX

Thank you for contributing to the **Tunisian Data Hub**! This project is the collective brain of the Tunisian AI ecosystem. By contributing, you are directly helping **3amAli** and other local models understand our dialect, our culture, and our daily reality.

---

## GETTING STARTED

### 1. SETUP

Fork the repository to your own GitHub account and clone it to your local machine:

```bash
# Clone the repository
git clone https://github.com/iyedex-labs/3amali-tunisian-data

# Enter the project directory
cd 3amali-tunisian-data

```

### 2. CHOOSE YOUR CATEGORY

Before adding data, browse the `data/` directory. Each folder has a specific purpose.

| IF YOU HAVE... | TARGET DIRECTORY |
| --- | --- |
| **Q&A / Chat Pairs** | `data/01_chat_darja/q_a_casual/` |
| **Jokes (Nokat)** | `data/02_humor_nokat/nokat_short/` |
| **Proverbs (Amthal)** | `data/03_wisdom_amthal/amthal_sha3biya/` |
| **Corporate Info** | `data/04_enterprise_economy/company_profiles/` |
| **History / Facts** | `data/05_knowledge_facts/history_timeline/` |

---

## STEP-BY-STEP SUBMISSION

### STEP 1: CREATE A FEATURE BRANCH

Always create a new branch for your specific contribution. This keeps the project history clean.

```bash
git checkout -b feat-add-sfaxi-proverbs

```

### STEP 2: PREPARE YOUR DATA

1. Create a new `.json` file inside the appropriate folder.
2. Name the file clearly (e.g., `tunis_street_talk_01.json`).
3. Ensure your data follows the formatting rules in `docs/metadata_standards.md`.

### STEP 3: COMMIT AND PUSH

Be descriptive in your commit messages so reviewers know what you added.

```bash
git add .
git commit -m "feat: added 30 classic Tunisian jokes to nokat_short"
git push origin feat-add-sfaxi-proverbs

```

### STEP 4: OPEN A PULL REQUEST (PR)

1. Navigate to the [iyedex-labs/3amali-tunisian-data](https://github.com/iyedex-labs/3amali-tunisian-data) repository.
2. Click the **"Compare & pull request"** button that appears at the top.
3. Provide a brief summary of your data source and the number of entries added.

---

## REVIEW GUIDELINES

The **IyedeX** team and community maintainers review every Pull Request. We look for:

1. **Authenticity**: Does the Darja sound natural? (Avoid literal Google Translate results).
2. **Structure**: Is the JSON schema correct? (No missing brackets or commas).
3. **Accuracy**: Is the factual information (History/Business) verified and public?
4. **Safety**: Does the content respect community guidelines? (No hate speech or private personal info).

---

## NEED HELP?

If you have a large dataset (thousands of rows) or you are unsure about where to place a specific type of data:

* Open an **Issue** with the label `question`.
* Contact the **IyedeX** team via the official community channels.
