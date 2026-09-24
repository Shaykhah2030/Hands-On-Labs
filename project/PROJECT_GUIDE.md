# 🚀 Final Project — Meeting Follow-up Assistant

**Program:** L0-FGP · Generative AI for Productivity · [SDAIA Academy](https://github.com/SDAIAAcademy)
**Weight:** 100% of your course evaluation · **Submitted on:** GitHub

---

## 📖 The scenario

You are the project coordinator for the **Customer Portal Launch** at *Nakheel Tech* (a fictional company).
The team just finished its weekly meeting. Your job: turn the meeting into a **clear, verified, safe follow-up**, and build a **personal AI assistant** that can do this again next week.

This project proves you can run a **complete, safe productivity workflow with generative AI**, not just write one prompt.

> ✅ You may use **any** AI tool you like (Gemini, ChatGPT, Copilot, Claude). You do **not** need to use every tool.
> What we assess is **your workflow and your judgment**, not how many apps you used.

---

## 📦 Your data pack *(all fictional)*

| File | What it is |
|---|---|
| [`01_meeting_transcript`](../data-pack/project/01_meeting_transcript.txt) (.txt / .pdf) | The weekly sync meeting |
| [`02_project_tasks_status.csv`](../data-pack/project/02_project_tasks_status.csv) | Task tracker: owners, due dates, status |
| [`03_project_guidelines.pdf`](../data-pack/project/03_project_guidelines.pdf) | The project's official rules |
| [`04_email_style_sample.pdf`](../data-pack/project/04_email_style_sample.pdf) | How follow-up emails should look |

---

## 🧭 The six steps

Save your work into the matching folder of your repository (see the [template](template/)).

### Step 1 · Extract what matters 🔍 → `prompts/` and `outputs/`
Write an **R-C-T-F prompt** that extracts from the transcript:
**decisions · tasks · owner of each task · due dates · open questions**.

- Save your **first** prompt and result, then your **improved** prompt and result (before → after).
- Rule: if an owner or date is missing, the output must say **"To be confirmed"**, never invent one.

### Step 2 · Write the follow-up email 📧 → `outputs/follow-up-email.md`
A professional email to all attendees containing: a short summary, decisions, actions (Owner – Task – Due), and open questions.
Follow the **style sample** (subject format, structure, tone, length).

### Step 3 · Read the data 📊 → `outputs/data-summary.md`
Upload the task-status CSV and get:
- **3 key indicators** with exact numbers
- **1 important pattern** or observation
- A **simple explanation** for a manager
- A **warning** about any conclusion the data does **not** support

⭐ **Bonus insight:** compare the CSV with the transcript. Do they agree on every owner and date?

### Step 4 · Verify against the sources 🔎 → `verification/source-checks.md`
Add the **guidelines** (and optionally the transcript) to **Gemini Notebook** *(formerly NotebookLM)*, then:
- Ask **2–3 questions** that test your outputs against the rules
- **Check the citations**
- **Correct** anything in your extraction or email that the sources don't support, or that breaks the rules

> 💡 Hint: read the guidelines carefully. Did the team agree to anything in the meeting that the rules don't allow?

### Step 5 · Build your personal assistant 🤖 → `assistant/`
Create a **Gem** in Gemini named **Meeting Follow-up Assistant** (or the equivalent in your tool). Its fixed instructions must:
1. Extract decisions and tasks **only** from the text provided
2. **Never invent** an owner or a date
3. Write **"To be confirmed"** when information is missing
4. Write a short, professional follow-up email
5. **Ask for clarification** when the input is incomplete
6. Follow the writing style in the reference file (attach the style sample)

**How to create a Gem:** open [gemini.google.com](https://gemini.google.com) → **Gems** → **New Gem** → add a name, instructions and knowledge files → **test it in the preview** → Save.
*Availability depends on your account and your organization's policy. If Gems aren't available to you, save the same instructions as a reusable prompt and test it in your chosen tool.*

**Test it** with the transcript and save a screenshot or a written description of the result.

### Step 6 · Safety review 🔐 → `verification/safety-review.md`
Fill in this table:

| Item | Your decision |
|---|---|
| Data used | Fictional or public? |
| Data removed before pasting | e.g., names, phone numbers, IDs (if any) |
| Sources verified | Which documents and citations did you check? |
| Connector permissions | Did you use any? Why? Were they removed? |
| What still needs human review | e.g., numbers, commitments, owners, tone |

---

## 📁 Step 7 · Publish on GitHub

Use the **[template](template/)** folder and follow the **[GitHub quick-start](GITHUB_QUICKSTART.md)**.

Your repository **must** include:
- [ ] A clear, complete **project description**
- [ ] A professional **README** explaining the idea and **how to use** your assistant
- [ ] **Technical documentation** in `docs/` (workflow, tools, limitations)
- [ ] **Good Git practice**: at least **one commit per step**, with clear messages
- [ ] A reference to the training program: **L0-FGP · Generative AI for Productivity**
- [ ] A link to **SDAIA Academy on GitHub**: https://github.com/SDAIAAcademy

---

## ⏱️ Timing (Day 3 afternoon)

| Activity | Time |
|---|---|
| Steps 1–6 | 60 min |
| Peer review (swap with a colleague and use the rubric below) | 15 min |
| Final edits + publish on GitHub | 20 min |
| Presentations (selected projects) | 2–3 min each |
| Post-test | 20 min |

---

## 📊 Assessment rubric (100%)

| # | Criterion | What earns full marks | Weight |
|---|---|---|---|
| 1 | Extraction | R-C-T-F prompt, clear before→after improvement, no invented owners or dates | 15% |
| 2 | Follow-up email | Complete, matches the style sample, correct subject format, right tone | 10% |
| 3 | Data insights | Correct numbers, a real pattern, a clear "not supported" warning | 15% |
| 4 | Source verification | Questions tested against the guidelines, citations checked, **rule conflicts found and corrected** | 15% |
| 5 | Personal assistant | All 6 instructions, tested, handles missing information properly | 15% |
| 6 | Safety review | Table complete and thoughtful; access removed where used | 10% |
| 7 | GitHub repository | README complete (incl. L0-FGP + SDAIA link), docs, meaningful commits, clean structure | 20% |

---

## 🌍 Give back to the community

As part of the SDAIA Academy ecosystem, please also:
- ⭐ **Star** high-quality Saudi projects you find useful
- 👤 **Follow** Saudi developers and organizations, including [SDAIA Academy](https://github.com/SDAIAAcademy)
- 🤝 **Contribute** to open-source projects when you can
- 🔁 Use **Fork**, **Pull Requests** and **Issues** to collaborate
- 📣 **Share** standout projects with your network
