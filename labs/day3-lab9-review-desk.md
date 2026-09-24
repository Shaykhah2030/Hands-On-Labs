# 🕵️ Day 3 · Lab 9 — The Review Desk

**Level:** 🟡 Practice &nbsp;·&nbsp; **Time:** ~25 min &nbsp;·&nbsp; **Tool:** your chosen AI tool

> Two parts:
> **A.** Catch the errors in an AI summary *(human review)*
> **B.** Make the AI stick to the facts *(grounding)*

---

## Part A · The Review Desk 🔎

Your manager asked an AI tool to summarize a report for the board. It *looks* great. But before it goes out, **you** are the reviewer.

📄 **The source report** *(fictional, and the only trusted source)*
```text
Nakheel Freight Q2 Operations Report. In Q2, the company delivered 48,200 shipments, up 12% from Q1. On-time delivery reached 94.5%. The Jeddah hub processed 21,000 shipments, the highest of all hubs. Customer complaints fell from 310 to 245. The company opened one new hub in Dammam in May. Fuel costs rose by 7% due to higher prices. The team plans to pilot electric vans in Q4.
```

🤖 **The AI's summary**
```text
Nakheel Freight delivered 48,200 shipments in Q2, a 12% increase over Q1. On-time delivery reached 97.5%, an all-time record. The Jeddah hub was the busiest, handling 21,000 shipments. Complaints dropped from 310 to 245. Two new hubs opened in Dammam and Riyadh in May. Fuel costs rose by 7%. According to the Saudi Logistics Council, the company is now the fastest-growing carrier in the region.
```

✏️ **Your task:** using the checklist below, find **every problem** in the summary. **Don't use AI for this part.** This is your human review skill. ⏱️ 5 minutes.

### ✅ Review checklist
- [ ] Every **number** matches the source
- [ ] Every **name / place** appears in the source
- [ ] No **claims** that go beyond the source ("record", "best", "fastest")
- [ ] No **new sources** the original never mentioned
- [ ] Nothing **important** is missing

<details>
<summary>🔒 <b>Answer key: 5 problems</b></summary>

| # | In the summary | The truth | Type |
|---|---|---|---|
| 1 | On-time delivery **97.5%** | **94.5%** | ❌ Wrong number |
| 2 | "an **all-time record**" | Not in the source | ⚠️ Unsupported claim |
| 3 | "**Two** new hubs" | **One** new hub | ❌ Wrong number (written as a word, so easy to miss!) |
| 4 | "Dammam **and Riyadh**" | Only Dammam | ❌ Invented place |
| 5 | "According to the **Saudi Logistics Council**… fastest-growing" | Not in the source | ❌ Invented source and claim |

Also missing: the **electric-van pilot in Q4**.

💡 Four of the seven sentences were perfect, which is exactly why the errors are easy to miss. **Fluent ≠ correct.**

</details>

---

## Part B · Make the AI stick to the facts 📌

Now let's see if a better prompt prevents those errors.

📋 **Step 1: a grounded summary**
```text
Act as a business analyst. Summarize the report below for the board in 5 bullet points. Use ONLY facts and numbers that appear in the report. Do not add opinions, records, comparisons or outside sources. If something is not in the report, do not mention it.

[paste the source report]
```

📋 **Step 2: ask it to show its evidence** (same chat)
```text
For each bullet point you wrote, quote the exact sentence from the report that supports it.
```

✏️ Run the Review checklist from Part A on the new summary.

👀 **Observe:** Did grounding + evidence reduce the errors? Could you verify each point faster?

<details>
<summary>🔒 <b>What you should notice</b></summary>

Grounded prompts usually produce **far fewer** invented details, and asking for supporting quotes makes checking much faster.
But it's **not a guarantee**. You still review before sending. The AI speeds up the checking; it doesn't replace you.

</details>

---

## 🏁 Wrap-up

```
✍️ Clear prompt (R-C-T-F)  →  🔁 Iterate  →  🔐 Protect the data  →  🔎 Review & verify  →  ✅ Use it
```

🚀 **Next:** your final project puts this whole workflow together.
