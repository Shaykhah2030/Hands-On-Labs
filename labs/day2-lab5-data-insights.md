# 📊 Day 2 · Lab 5 — From Spreadsheet to Insight

**Level:** 🟢 Starter &nbsp;·&nbsp; **Time:** ~40 min &nbsp;·&nbsp; **Tool:** your chosen AI tool (Gemini, ChatGPT, Copilot or Claude)

> You're a help-desk team lead. Your manager wants to know **how Q2 went**, in plain language, by tomorrow.
> You have a spreadsheet of **150 support tickets** *(fictional data)*. Let's turn it into insight, and **check every number**.

🎥 **First, your trainer will show** how AI works *inside* spreadsheets (Gemini in Google Sheets, Copilot in Excel).
Those features require an eligible account or licence, so in this lab we'll do the same thing with a free chat tool.

---

## 📥 Get the data

1. Download 👉 [`helpdesk_tickets_q2_2026.csv`](../data-pack/lab5-data/helpdesk_tickets_q2_2026.csv)
2. In your AI tool, click the **attach / ➕ / 📎** button and upload the file.

> 💡 **Can't upload files in your tool?** Open the CSV in Notepad or TextEdit, copy everything, and paste it after your prompt. A CSV is just text.

**The columns:** `ticket_id` · `date` · `category` · `priority` · `channel` · `resolution_hours` · `satisfaction_1to5` · `status`

---

## Round 1 · Understand the data before analysing it 🔍

📋
```text
Describe this dataset before analysing it: how many rows, what each column means, the date range, and whether any values are missing. Do not draw conclusions yet.
```

👀 **Check:** Did it count **150 rows**? Did it notice that some **satisfaction** and **resolution time** values are empty? Why might they be empty?

<details>
<summary>🔒 <b>Answer</b></summary>

- 150 tickets, from April to June 2026.
- **Open** tickets have no resolution time or rating yet, because they aren't finished.
- Some **closed** tickets have no rating, because the customer didn't rate them (12 tickets).

💡 Starting with *"describe the data"* catches misunderstandings early, before they turn into wrong conclusions.

</details>

---

## Round 2 · Three key indicators 🎯

📋
```text
Act as a data analyst. Using only this file, give me:
1. Three key indicators with exact numbers
2. One important pattern or trend
3. A simple explanation for a non-technical manager (max 3 sentences)
4. A warning about any conclusion this data does NOT support
```

✏️ **Now verify.** Compare the AI's numbers with the answer key. Are they exact?

<details>
<summary>🔒 <b>Answer key (calculated directly from the file)</b></summary>

| Indicator | Correct value |
|---|---|
| Total tickets | 150 (144 closed, 6 open) |
| Top category | Password reset: 73 tickets (48.7%) |
| Avg resolution time by month | April 8.0 h → May 5.4 h → June 4.4 h |
| Slowest category | Network: 21.0 h on average |
| Satisfaction by channel | Phone 4.18 · Portal 3.90 · Email 3.51 |
| Overall avg satisfaction | 3.83 / 5 (rated tickets only) |
| High-priority tickets | 21 |

⚠️ AI tools sometimes **round, miscount or estimate** instead of calculating. If a number is off, ask: *"Show me how you calculated this."*

</details>

---

## Round 3 · The "why" trap ⚠️

📋
```text
Why did the average resolution time drop from April to June?
```

👀 **Observe:** Did the AI give you **reasons**, like new staff, a new tool, or better training?

<details>
<summary>🔒 <b>What you should notice</b></summary>

The file has **no column** about staff, tools or training. Any "reason" the AI gives is a **guess presented as a fact**.

✅ **Better prompt:**

```text
Based ONLY on this data, what can and cannot be concluded about why resolution time dropped? List possible explanations separately and clearly label them as hypotheses that need checking.
```

**Data tells you *what* happened. It rarely tells you *why*.** That part needs a human who knows the context.

</details>

---

## Round 4 · Make it ready for your manager 📋

Stay in the same chat.

📋 **A table**
```text
Create a table of tickets per category with count and percentage, sorted from highest to lowest.
```

📋 **A 3-bullet summary**
```text
Write a 3-bullet summary of Q2 for the IT manager: one good result, one concern, and one recommended action. Use exact numbers from the file.
```

✏️ **Check** the numbers in both outputs against the answer key one last time.

💬 **Discuss:** 49% of tickets are password resets. What would you recommend? (e.g., a self-service password reset tool)

---

## 🧠 Quick quiz

**Q1.** What's the best first prompt when you upload a new dataset?
A) "Analyze this"  B) "Describe the data: rows, columns, missing values"  C) "Make a chart"  D) "Give me insights"

<details><summary>🔒 Answer</summary>

**B.** Understand the data first, then analyse it.

</details>

**Q2.** The AI says satisfaction rose "because of the new chatbot". The file has no chatbot column. This is:
A) A verified insight  B) An unsupported guess  C) A calculation  D) A data error

<details><summary>🔒 Answer</summary>

**B. An unsupported guess.** Label it as a hypothesis, or remove it.

</details>

---

📚 **Save it:** add your Round 2 prompt to `my-prompts.md`. It works for almost any spreadsheet.
