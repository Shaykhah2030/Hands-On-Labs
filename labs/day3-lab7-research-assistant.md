# 📚 Day 3 · Lab 7 — Your AI Research Assistant

**Level:** 🟢 Starter &nbsp;·&nbsp; **Time:** ~40 min &nbsp;·&nbsp; **Tool:** Gemini Notebook *(formerly NotebookLM)* + your chosen AI tool

> A normal AI chat answers from its **general training**. A research assistant answers from **your sources**, and shows you *where* each answer came from.
> That's the difference between *"sounds right"* and *"I can prove it."*

> ℹ️ **Name change:** in July 2026 Google renamed **NotebookLM** to **Gemini Notebook**. It's the same product, and the old address `notebooklm.google.com` still works.

---

## 📥 Setup (5 min)

1. Download the 3 fictional company policies from [`data-pack/lab7-research-sources`](../data-pack/lab7-research-sources/):
   `Travel_Policy.pdf` · `Remote_Work_Policy.pdf` · `IT_Security_Guidelines.pdf`
2. Open [notebooklm.google.com](https://notebooklm.google.com) and sign in with your **personal** Google account
3. Create a **new notebook** and **add the 3 PDFs** as sources

---

## Round 1 · Ask, then check the citation 🔎

Ask each question. After each answer, **click the citation numbers** and read the original text.

📋
```text
How many days per week can I work remotely, and when do I become eligible?
```
📋
```text
Can I paste an internal company report into a free public AI tool to summarize it?
```
📋
```text
What is the daily per diem for an international trip, and how long do I have to submit my expense claim?
```

<details>
<summary>🔒 <b>Answers (check against your citations)</b></summary>

| Question | Answer | Source |
|---|---|---|
| Remote work | Up to **2 days/week**, after the **6-month probation** | Remote Work Policy §1–2 |
| Internal report in a public AI tool | **Not allowed.** Internal data only goes into the company-approved internal assistant | IT Security Guidelines §3 |
| International trip | **SAR 750/day**; claim within **10 working days** | Travel Policy §4–5 |

</details>

---

## Round 2 · Connect the documents 🧩

📋
```text
I want to work remotely from a café on Monday. List every rule from these documents that applies to me, and cite each one.
```

<details>
<summary>🔒 <b>Answer</b></summary>

- ❌ **Not on Monday.** Mondays are in-office team days (Remote Work §2).
- On other days: company laptop only, **VPN on at all times**, and public Wi-Fi only with the VPN (Remote Work §4).
- Be available on Teams **9:00–13:00** (Remote Work §3).
- Lock your screen when you step away; it auto-locks after 5 minutes (IT Security §2).

💡 A good answer combines **two documents** and catches the **Monday** rule.

</details>

---

## Round 3 · The trap question 🪤

📋
```text
What is the monthly parking allowance for employees?
```

👀 **Observe:** None of the documents mention parking. A good research assistant should say **it can't find this in the sources**, not invent an amount.

---

## Round 4 · Same question, no sources ⚖️

Now open your **normal AI chat** (no documents attached) and ask:

📋
```text
What is the daily per diem for an international business trip at Nakheel Tech?
```

👀 **Compare:** Did the normal chat admit it doesn't know this fictional company, or did it give a **generic or invented** answer?

<details>
<summary>🔒 <b>The lesson</b></summary>

Without your sources, the AI can only guess from general knowledge. **Grounding** (giving the AI your documents and asking for citations) is the most reliable way to reduce made-up answers at work.

</details>

---

## Round 5 · Turn sources into something useful 🛠️

📋
```text
Create a one-page FAQ for new employees with the 6 most important rules from these documents. Keep each answer to one sentence and cite the source for each.
```

✏️ Pick **two** FAQ answers at random and check their citations. Are they accurate?

---

## 🧰 Research techniques cheat-sheet

| # | Technique | Prompt idea |
|---|---|---|
| 1 | **Ground it** | Upload the sources; ask it to answer *only* from them |
| 2 | **Demand evidence** | *"Cite the source for each point"*, then click and read |
| 3 | **Ask what's missing** | *"What does this question need that is NOT in the sources?"* |
| 4 | **Separate fact from opinion** | *"Label each point as stated fact or your interpretation"* |
| 5 | **Cross-check** | Ask a second tool or a colleague about important claims |
| 6 | **Go to the original** | For decisions, always read the original source yourself |

🎥 **Trainer demo:** *Deep Research* browses many websites and writes a cited report. Availability and limits depend on your plan. Even then, **technique 6 still applies.**

---

## 🧠 Quick quiz

**Q1.** What makes a source-grounded tool like Gemini Notebook more reliable for company policies?
A) It's faster  B) It answers from your uploaded sources and shows citations  C) It never makes mistakes  D) It uses more languages

<details><summary>🔒 Answer</summary>

**B.** It still can make mistakes, which is why you click and check the citations.

</details>

**Q2.** The tool can't find an answer in your sources. What's the best behaviour?
A) Invent a likely answer  B) Say it isn't in the sources  C) Answer from general knowledge without saying so  D) Refuse to answer anything else

<details><summary>🔒 Answer</summary>

**B.** "Not in the sources" is a **good** answer. It tells you where the gap is.

</details>
