# 🛡️ Day 3 · Lab 8 — Safe or Not Safe?

**Level:** 🟢 Starter &nbsp;·&nbsp; **Time:** ~30 min &nbsp;·&nbsp; **Tool:** your chosen AI tool

> Using AI **well** also means using it **safely**. In this lab you'll practise two habits that protect you and your organization:
> 1. 🔐 **Protect the data** before you paste it
> 2. 🔎 **Check the facts** before you use them

---

## Part A · Safe to paste? 🚦

For each situation, decide: **🟢 Safe**, **🟡 Redact first**, or **🔴 Never paste into a public AI tool**.
Write your answers down, then reveal.

| # | Situation |
|---|---|
| 1 | A press release your company already published on its website |
| 2 | A customer complaint that contains the customer's name, phone number and national ID |
| 3 | Your company's unreleased quarterly financial results |
| 4 | Your own CV, which you want to improve before applying for jobs 🎓 |
| 5 | A server password that "isn't working" and you want help troubleshooting |
| 6 | A general question: "How do I write a good project status report?" |
| 7 | An internal HR investigation report about an employee |
| 8 | Meeting notes about a public training event, with no personal details |

<details>
<summary>🔒 <b>Answers</b></summary>

| # | Answer | Why |
|---|---|---|
| 1 | 🟢 Safe | It's already public |
| 2 | 🟡 Redact first | Remove the name, phone number and ID, and the AI can still help draft a reply |
| 3 | 🔴 Never | Confidential business information |
| 4 | 🟡 Redact first | Your own data, but remove your phone number, ID and address. The AI doesn't need them |
| 5 | 🔴 Never | Credentials must never be shared, even "partially" |
| 6 | 🟢 Safe | No data at all, only a question |
| 7 | 🔴 Never | Highly sensitive personal and confidential information |
| 8 | 🟢 Safe | Public, no personal data |

💡 **Rule of thumb:** if you'd be uncomfortable seeing it posted on a public website, don't paste it into a public AI tool.
Some organizations provide **approved internal AI tools** with stronger protections. Always follow your organization's policy.

</details>

---

## Part B · Redact it yourself ✂️

A colleague wants AI help replying to this complaint *(fictional data)*:

```text
Subject: Complaint about delayed refund

Hello, my name is Khalid Al-Harbi. I ordered on 3 March and still have not received my refund of SAR 1,200.
You can reach me at khalid.harbi88@examplemail.com or on 0551234567.
My national ID is 1098765432 and my refund should go to IBAN SA0380000000608010167519.
Please resolve this quickly, or I will escalate. Thanks, Khalid
```

✏️ **Step 1:** Copy the complaint into your notes app (**not** the AI tool!) and replace every piece of personal data with a label such as `[NAME]`, `[EMAIL]`, `[PHONE]`, `[ID]`, `[IBAN]`.

> ⚠️ Don't ask the AI to redact it for you. That would mean pasting the personal data into the AI tool, which is exactly what we're trying to avoid.

<details>
<summary>🔒 <b>Redacted version</b></summary>

```text
Subject: Complaint about delayed refund

Hello, my name is [NAME]. I ordered on 3 March and still have not received my refund of SAR 1,200.
You can reach me at [EMAIL] or on [PHONE].
My national ID is [ID] and my refund should go to IBAN [IBAN].
Please resolve this quickly, or I will escalate. Thanks, [NAME]
```

✅ The date and the amount can stay. They're needed for the reply and don't identify the person.

</details>

✏️ **Step 2:** Now paste your **redacted** version into the AI tool with this prompt:

📋
```text
Act as a customer service specialist. Draft a polite, apologetic reply to the complaint below. Promise a response within 2 working days and keep the placeholders like [NAME] exactly as they are so I can fill them in later. Under 120 words.

[paste your redacted complaint]
```

👀 **Observe:** The AI helped fully, **without ever seeing Khalid's data**. You fill in the name yourself before sending.

---

## Part C · Catch the made-up facts 🔎

📋 Run this prompt:
```text
Give me 5 statistics about how many hours per week employees in Saudi Arabia spend on email, with the source for each statistic.
```

✏️ Now pick **two** of the statistics and try to find the original source (search for the source name + the number).

👀 **Record in your notes:**

| Statistic | Source the AI gave | Could I find it? ✅ / ❌ |
|---|---|---|
| | | |
| | | |

<details>
<summary>🔒 <b>What you should notice</b></summary>

Very specific statistics about narrow topics are **hallucination hotspots**. The AI may:
- invent a number that sounds reasonable,
- attribute a real statistic to the wrong source, or
- cite a source that doesn't exist.

✅ **Better prompt:** ask the AI to say when it's unsure, and to separate facts from estimates:

```text
What is known about how much time employees spend on email? Clearly separate (1) findings from well-known published studies and (2) your general estimates. If you are not sure a source exists, say so instead of guessing.
```

Even then: **verify before you publish.**

</details>

---

## 🧠 Quick quiz

**Q1.** What's the safest way to get AI help with a document containing personal data?
A) Paste it and delete the chat afterwards  B) Remove the personal data yourself first, then paste  C) Ask the AI to remove the personal data  D) Paste only half of it

<details><summary>🔒 Answer</summary>

**B.** Redact **before** the data leaves your hands. Deleting a chat afterwards doesn't guarantee the data was never stored or processed.

</details>

**Q2.** The AI gives you a statistic with a source. What's the right next step?
A) Use it, since it has a source  B) Ask the AI "is this correct?"  C) Find and check the original source yourself  D) Round the number

<details><summary>🔒 Answer</summary>

**C.** Only the original source can confirm the number.

</details>

---

📚 **Save it:** add the "separate facts from estimates" prompt to `my-prompts.md`. It's a great safety habit.
