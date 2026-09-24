# 💇 Day 1 · Lab 2 — Prompt Makeover

**Level:** 🟡 Practice &nbsp;·&nbsp; **Time:** ~45 min &nbsp;·&nbsp; **Tool:** your chosen AI tool

> In Lab 1 the prompts were ready-made. Now **you write them.**
> Each weak prompt below comes with the facts you need. Your job is to give it an **R-C-T-F makeover**.

---

## ✅ Your prompt checklist

Before you run any prompt, check it:

- [ ] 👤 **Role:** who should the AI act as?
- [ ] 📚 **Context:** did I give the facts it can't guess (who, what, when, why)?
- [ ] 🎯 **Task:** does it start with a clear action verb (Write, Summarize, List, Explain…)?
- [ ] 📐 **Format:** did I set the length, structure or tone?

---

## Part A · Three makeovers ✏️

For each case:
1. Run the **weak prompt** as it is.
2. Write your **improved prompt** using the facts given.
3. Run it and compare.
4. Then reveal the model prompt 🔒. There's no single right answer, so compare ideas.

---

### Case 1 · 💼 "Summarize this."

**Facts:** You're an IT team lead. Five interns start next week. You want them to understand this policy quickly:

📋 *(paste this text after your prompt)*
```text
IT Acceptable Use Policy (extract): Employees must lock their screens when leaving their desks. Passwords must be at least 12 characters and changed every 90 days. Personal USB drives are not permitted on company devices. Company data must not be uploaded to personal cloud storage or public AI tools without approval from the IT Security team. Suspected phishing emails must be reported using the "Report Phishing" button and must not be forwarded. Violations may result in suspended system access.
```

❌ **Weak prompt:** `Summarize this.`

<details>
<summary>🔒 <b>Model prompt</b></summary>

```text
Act as an IT security trainer. Five new interns start next week and need to understand our IT policy quickly. Summarize the policy below into the 5 most important rules, each as one short "Do" or "Don't" sentence in simple language. Add one line at the end explaining what happens if the rules are broken.

[paste policy]
```

</details>

---

### Case 2 · 🎓 "Write a job application."

**Facts:** You're applying for a **Junior Data Analyst** role at *Nakheel Tech* (fictional). You have a bachelor's in Computer Science, know SQL, Python and Power BI, and built a graduation project analysing hospital wait times.

❌ **Weak prompt:** `Write a job application.`

<details>
<summary>🔒 <b>Model prompt</b></summary>

```text
Act as a career coach who helps fresh graduates in Saudi Arabia. I am applying for a Junior Data Analyst position at Nakheel Tech. I have a bachelor's degree in Computer Science and skills in SQL, Python and Power BI. My graduation project analysed hospital patient wait times to recommend scheduling improvements. Write a cover letter that connects my project to the role. Keep it under 200 words, confident but not exaggerated, in formal English.
```

⚠️ Always check that the AI didn't **invent** experience or skills you don't have.

</details>

---

### Case 3 · 💼🎓 "Explain APIs."

**Facts:** Your HR manager (non-technical) asked why the new HR system needs an "API" to connect with the payroll system.

❌ **Weak prompt:** `Explain APIs.`

<details>
<summary>🔒 <b>Model prompt</b></summary>

```text
Act as a friendly IT specialist. My HR manager has no technical background and asked why our new HR system needs an "API" to connect to the payroll system. Explain what an API is using one everyday analogy, and why it helps HR and payroll share data. Maximum 100 words, no technical jargon.
```

💡 Being able to explain technical ideas simply is a valuable job skill, and AI is a great practice partner for it.

</details>

---

## Part B · Show, don't just tell: using an example 🧩

Sometimes describing a style is hard. It's easier to **show an example**.

📋 Run this prompt:
```text
Write 3 short LinkedIn post headlines announcing that I completed a course on Generative AI for Productivity.

Here is an example of the style I like:
"3 days, 1 big shift: how I now write emails in half the time 🚀"
```

✏️ Now replace the example with a **different style** (e.g., formal, or in Arabic) and run it again.

👀 **Observe:** How closely did the AI copy the style of your example: length, emoji, structure?

---

## Part C · Iteration challenge 🔁

**Goal:** In **maximum 4 messages** in the same chat, get this result:

> A bilingual (Arabic + English) announcement, **under 50 words per language**, inviting colleagues to a "Lunch & Learn" on AI tools this Wednesday at 12:30 in Meeting Room 3.

Start with a simple prompt and improve it step by step. Count your messages!

<details>
<summary>🔒 <b>Example path</b></summary>

1. `Write an invitation to a Lunch & Learn session about AI tools, Wednesday 12:30, Meeting Room 3.`
2. `Make it under 50 words and more energetic.`
3. `Now add an Arabic version below it, also under 50 words.`

✅ 3 messages. Each message changed **one thing**, which is the fastest way to steer.

</details>

---

## 💬 Reflect

- Which case was the hardest to improve? Which ingredient was missing?
- In the class comparison, did different tools give different results for the same prompt?

📚 **Save it:** copy your **two best prompts** from this lab into `my-prompts.md`, with one line explaining when you'd use each.
