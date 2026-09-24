# 🗂️ Day 2 · Lab 4 — From Meeting Chaos to Action Plan

**Level:** 🟡 Practice &nbsp;·&nbsp; **Time:** ~50 min &nbsp;·&nbsp; **Tool:** your chosen AI tool

> You just left the **Project Falcon** kickoff meeting (launching an internal HR chatbot 🤖).
> It was messy: people arrived late, went off-topic, and made decisions mid-conversation.
> Your manager wants a **clear follow-up by the end of the day.** This time, **you write every prompt.** ✏️
>
> 🔁 This is a **guided rehearsal** for your final project, which uses a different meeting.

---

## 📜 The meeting notes *(fictional)*

📋 Copy the full transcript. You'll paste it into your prompts.
```text
Project Falcon kickoff — Sunday 9:00 AM
Sara (Project Manager): Okay everyone, let's start. The goal today is to lock the launch plan for Falcon.
Omar (Procurement): The vendor finally sent the pricing, it's within budget. I think we should just go with their standard package, the premium one isn't worth it.
Sara: Agreed, let's go with the standard package.
Lina (HR): Before we go further — has Legal approved the data policy? We can't launch without it.
Sara: Good point, nobody has confirmed that yet.
Omar: I'll send the signed contract to the vendor by Tuesday.
Lina: I can prepare the training material for HR staff, I'll have the deck ready by Thursday.
Faisal (IT): Sorry I'm late, traffic was terrible. Did I miss anything?
Sara: We picked the standard package. We still need a pilot group.
Faisal: What about the finance team? They're small and they complain the most about HR requests, haha.
Sara: Perfect, finance it is. Faisal, can you schedule the pilot kickoff with them? Let's say by next Sunday.
Faisal: Sure.
Omar: One more thing — who is going to own support after launch? IT or HR?
Sara: Let me check with the directors and confirm by Wednesday.
Lina: Also, the cafeteria has new coffee. Just saying.
Sara: Great, thanks all. Meeting closed at 9:30.
```

---

## Task 1 · Extract the key information 🔍

✏️ Write a prompt that turns the transcript into **three clear sections**:
1. **Decisions** made
2. **Action items** as a table: *Owner · Task · Deadline*
3. **Open questions**

<details>
<summary>💡 <b>Hint</b></summary>

Use R-C-T-F. Tell the AI exactly which sections and table columns you want, and ask it to **ignore off-topic chat**.

</details>

<details>
<summary>🔒 <b>Model prompt</b></summary>

```text
Act as an executive assistant. Below is the transcript of our Project Falcon kickoff meeting (launching an internal HR chatbot). Extract:
1. Decisions made
2. Action items as a table with columns: Owner, Task, Deadline
3. Open questions that still need an answer
Ignore small talk and off-topic comments. Only use information stated in the transcript; if a deadline is not mentioned, write "Not stated".

[paste transcript]
```

</details>

### ✅ Verify the AI's answer

Compare the AI's result with the answer key. **Did it miss anything, or invent anything?**

<details>
<summary>🔒 <b>Answer key</b></summary>

**Decisions**
- Go with the vendor's **standard** package
- The pilot group will be the **finance team**

**Action items**

| Owner | Task | Deadline |
|---|---|---|
| Omar | Send the signed contract to the vendor | Tuesday |
| Lina | Prepare the HR staff training deck | Thursday |
| Faisal | Schedule the pilot kickoff with finance | Next Sunday |
| Sara | Confirm who owns post-launch support | Wednesday |

**Open questions**
- Has Legal approved the data policy? *(no owner assigned!)*
- Who owns support after launch: IT or HR? *(Sara is checking)*

⚠️ **Watch out for:**
- Did the AI assign the Legal question to someone? Nobody took it. An AI that invents an owner is **hallucinating**.
- Did the coffee ☕ or the "traffic" sneak into your notes?

</details>

---

## Task 2 · Write the follow-up email 📧

✏️ Using the result from Task 1 (stay in the same chat), write a prompt for a follow-up email to **all attendees**.
Requirements: under 150 words, a clear subject line, action items with owners and deadlines, and a polite nudge that the Legal question **needs an owner**.

<details>
<summary>🔒 <b>Model prompt</b></summary>

```text
Using the decisions, action items and open questions above, write a follow-up email from Sara to all meeting attendees. Include a clear subject line, a one-line thank-you, the decisions, the action items as a short list (owner – task – deadline), and ask who will follow up with Legal on the data policy. Under 150 words, professional and friendly.
```

</details>

---

## Task 3 · The executive summary 🎯

The HR Director wasn't in the meeting and has **30 seconds** to read your update.

✏️ Write a prompt for an update of **exactly 3 bullet points plus 1 risk line**.

<details>
<summary>🔒 <b>Model prompt</b></summary>

```text
Act as a project manager reporting to the HR Director, who has 30 seconds to read this. Based on the meeting information above, write exactly 3 bullet points covering progress, decisions and next steps, then one line starting with "Risk:" describing the biggest risk to the launch.
```

👀 The biggest risk should be the **Legal approval**. Did the AI spot it?

</details>

---

## Task 4 · Plan the next steps 📅

Choose your track:

**💼 Employed:** ✏️ Ask the AI to create an **agenda for next week's follow-up meeting** (30 minutes, with time per item), based on the open questions and action items.

**🎓 Preparing for a job:** ✏️ Ask the AI to turn this meeting into a **"project coordination" example you could talk about in an interview**, using the STAR method.

<details>
<summary>🔒 <b>Model prompts</b></summary>

💼
```text
Create a 30-minute agenda for next week's Project Falcon follow-up meeting. Base it on the open action items and questions above. Give each agenda item a time slot, an owner, and the expected outcome. Put the Legal data-policy approval first.
```

🎓
```text
I want to practise describing teamwork in interviews. Using this meeting as an example, help me write a short STAR story (Situation, Task, Action, Result) about coordinating a project kickoff where tasks needed clear owners and deadlines. Under 120 words, first person, realistic — do not exaggerate.
```

</details>

---

## 🏆 Bonus challenge · Real meetings are messier

Real transcripts are longer and in mixed languages. Ask the AI to write a **realistic 15-line meeting transcript in Arabic** about planning a company event, **with at least 3 hidden action items**.
Then swap transcripts with your neighbour and extract each other's action items. Who found them all? 🕵️

---

## 💬 Reflect

- Where did the AI save you the most time: extracting, writing, or planning?
- What did **you** have to check or fix by hand?

📚 **Save it:** add your Task 1 extraction prompt to `my-prompts.md`. It works for almost any meeting.
