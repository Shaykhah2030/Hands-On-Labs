# 🎮 Day 1 · Lab 1 — Prompt Playground

**Level:** 🟢 Starter &nbsp;·&nbsp; **Time:** ~30 min &nbsp;·&nbsp; **Tool:** pick ONE: Gemini, ChatGPT, Microsoft Copilot or Claude

> Every prompt in this lab is **ready-made**. Copy it 📋, paste it into your AI tool, and 👀 compare the results.
> The goal is to **see for yourself** what makes a prompt work.

> 🗳️ **Pick one tool and stay with it for this lab.** Your trainer will show the same prompts in the other tools, so the whole class can compare the results together.

**Tip:** start a **new chat** for each round, so earlier answers don't influence the next one.

---

## Round 1 · Vague vs. clear 🇬🇧

Run both prompts, each in a new chat.

📋 **Prompt A (vague)**
```text
Write an email about the meeting.
```

📋 **Prompt B (clear)**
```text
Act as an executive assistant. Our weekly team meeting has moved from Sunday 10 AM to Monday 11 AM because the manager is travelling. Write a short email to the 8 team members announcing the change. Keep it under 80 words, friendly and professional, with a clear subject line.
```

👀 **Observe**
- Did Prompt A's email contain **placeholders** like `[Date]` or details the AI had to *guess*?
- Which email could you send **right now** with the fewest edits?

<details>
<summary>🔒 <b>What you should notice</b> (click to reveal)</summary>

Prompt A usually gives a generic email full of `[brackets]` or invented details, because the AI doesn't know which meeting, when, or for whom.
Prompt B gives an email that is almost ready to send. The only change is that you **gave the AI the information it can't guess**.

</details>

---

## Round 2 · Same lesson, in Arabic 🇸🇦

📋 **البرومبت أ (غير واضح)**
```text
اكتب إعلان عن الدورة.
```

📋 **البرومبت ب (واضح)**
```text
تصرّف كمنسّق تدريب في جهة حكومية. لدينا دورة بعنوان «الذكاء الاصطناعي التوليدي لرفع الإنتاجية» لمدة 3 أيام، تبدأ يوم الأحد القادم من 9 صباحًا حتى 3 مساءً، وهي مناسبة للمبتدئين. اكتب إعلانًا قصيرًا يدعو الموظفين للتسجيل. الصيغة: أقل من 100 كلمة، بأسلوب رسمي ومشجّع، مع 3 نقاط توضّح فوائد الدورة.
```

👀 **Observe:** Does the pattern from Round 1 repeat in Arabic?

<details>
<summary>🔒 <b>What you should notice</b></summary>

Yes. **R-C-T-F works in any language.** The clear prompt gives a usable announcement with the right dates and length. The vague one invents a course.

</details>

---

## Round 3 · The power of **Role** 👤

Same task, three roles. Run each one in a new chat.

📋
```text
Act as a primary school teacher talking to 10-year-olds. Explain what generative AI is in 3 sentences.
```
📋
```text
Act as a senior software engineer talking to developers. Explain what generative AI is in 3 sentences.
```
📋
```text
Act as a business consultant talking to company managers. Explain what generative AI is in 3 sentences.
```

👀 **Observe:** How did the vocabulary, examples and tone change? Which version would you use in a job interview? 🎓

---

## Round 4 · The power of **Format** 📐

Same question, three formats.

📋
```text
أعطني نصائح لإدارة الوقت في العمل. الصيغة: 5 نقاط قصيرة.
```
📋
```text
أعطني نصائح لإدارة الوقت في العمل. الصيغة: جدول من عمودين: النصيحة، ومثال تطبيقي.
```
📋
```text
أعطني نصائح لإدارة الوقت في العمل. الصيغة: جملة واحدة فقط.
```

👀 **Observe:** You didn't change the question, only the format. Which result would you paste into a presentation slide?

---

## Round 5 · Test the limits ⚠️

AI tools are powerful, but they have limits. Let's find one.

📋
```text
Give me 3 academic studies about the effect of generative AI on employee productivity in Saudi companies. For each one, include the authors, the year, the journal, and a link.
```

✏️ **Now verify:** open each link, or search for each title.

👀 **Observe**
- Do all the links work?
- Do the studies really exist, with those exact authors and titles?

<details>
<summary>🔒 <b>What you should notice</b></summary>

Often at least one reference is **wrong or completely invented**. The title sounds real but doesn't exist, the link is broken, or the authors are mismatched.
This is called a **hallucination**: the AI produces text that *sounds* right, not text it has *checked*.

✅ **The lesson:** AI is excellent for drafts and ideas. **Facts, numbers and sources must always be verified.** (We'll practise this on Day 3.)

</details>

---

## Round 6 · Iterate: it's a conversation 🔁

This time, stay in the **same chat** for all three messages.

📋 **Message 1**
```text
Write a message to my team reminding them to submit their weekly reports.
```
📋 **Message 2**
```text
Make it shorter and more polite.
```
📋 **Message 3**
```text
Add a deadline: Thursday at 2 PM. Then give me an Arabic version too.
```

👀 **Observe:** You didn't start over. You *steered* the first draft. The first answer is a starting point, not the final product.

---

## ✏️ Round 7 · Your turn

Take the prompt below and change **the role and the format** at least twice. Try your own ideas, in English or Arabic.

📋
```text
Act as a friendly HR specialist. A new colleague joins our engineering team next Sunday. Write a welcome message for them. Format: 3 bullet points, under 60 words.
```

💡 Ideas: *"a strict school principal"*, *"a funny stand-up comedian"*, *"مدير موارد بشرية"*, *"a table"*, *"one short paragraph in Arabic"*

---

## 🧠 Quick quiz

**Q1.** The prompt *"Write an email about the meeting."* contains which R-C-T-F ingredient?
A) Role  B) Task  C) Format  D) Context

<details><summary>🔒 Answer</summary>

**B) Task.** "Write an email" is the only ingredient. There is no role, no context, and no format.

</details>

**Q2.** In Round 3, what made the three answers sound so different?
A) The format  B) The language  C) The role  D) Nothing changed

<details><summary>🔒 Answer</summary>

**C) The role.** The task and format stayed the same; only the "person" answering changed.

</details>

**Q3.** In Round 5, what should you do before using AI-generated references in a report?
A) Nothing, they look professional  B) Verify each one exists and says what the AI claims  C) Remove the links  D) Ask the AI if it is sure

<details><summary>🔒 Answer</summary>

**B) Verify each one.** Asking the AI "are you sure?" is not verification. It can confidently confirm its own mistakes.

</details>

---

## 🏁 Wrap-up

| Ingredient | What it does | Example |
|---|---|---|
| 👤 **Role** | Sets the voice and expertise | *Act as an HR specialist* |
| 📚 **Context** | Gives the facts the AI can't guess | *Meeting moved to Monday 11 AM* |
| 🎯 **Task** | Says exactly what to do | *Write an email to the team* |
| 📐 **Format** | Shapes the result | *Under 80 words, 3 bullet points* |

📚 **Save it:** copy your favourite prompt from Round 7 into `my-prompts.md`.
