# 🔌 Day 2 · Lab 6 — Connect AI to Your Files (Safely)

**Level:** 🟡 Practice &nbsp;·&nbsp; **Time:** ~35 min &nbsp;·&nbsp; **Tool:** Claude (free plan works) + Google Drive

> Until now, you copied and pasted content into the AI. A **connector** lets the AI **search, read and save files** in your apps directly.
> That's powerful, and it's exactly why we'll practise it **safely**: with a test folder, fictional files, and removing access at the end.

---

## ✅ Before you start

| You need | Notes |
|---|---|
| A **Claude** account | [claude.ai](https://claude.ai). The free plan includes the Google Drive connector |
| A **personal** Google account | ⚠️ Avoid your work account. Some organizations block this connection until an admin approves it |
| The **test files** | Download the 3 files in [`data-pack/lab6-drive-test-folder`](../data-pack/lab6-drive-test-folder/) |

**Prepare your test folder:**
1. Open [Google Drive](https://drive.google.com) → **New → Folder** → name it `AI-Lab-Test`
2. Upload the 3 files into it: `Travel_Policy.pdf`, `Team_Offsite_Notes.pdf`, `helpdesk_tickets_q2_2026.csv`

> 🔐 **Golden rule:** only ever connect to accounts and folders containing data you'd be comfortable sharing. Today, that's fictional data only.

---

## Step 1 · Connect 🔗

1. In Claude, open **Customize → Connectors**
2. Find **Google Drive** → click **Connect**
3. Sign in with your **personal** Google account
4. 👀 **Stop and read the permissions screen** before you click Allow

💬 **Discuss:** What is Claude asking to be allowed to do? Is that more than you need for this lab?

---

## Step 2 · Find an answer in your files 🔎

📋
```text
Search my Google Drive folder "AI-Lab-Test". What is the approved budget for the support team offsite, and how many people are attending?
```

👀 **Check:** Did Claude show **which file** it used? Click the source link and confirm.

<details>
<summary>🔒 <b>Answer</b></summary>

**SAR 60,000** approved budget · **18** attendees (from `Team_Offsite_Notes.pdf`).

</details>

---

## Step 3 · Connect information across files 🧩

This is where connectors shine: the AI can combine **two documents** for you.

📋
```text
Compare the hotel quote in Team_Offsite_Notes with the maximum domestic hotel rate in Travel_Policy. Is it within policy? Calculate the total hotel cost for all rooms and how much of it is above the policy limit. Show your calculation.
```

✏️ **Verify the maths yourself**, even if it looks right.

<details>
<summary>🔒 <b>Answer</b></summary>

- Quote: **SAR 1,100** per room per night · Policy maximum (domestic): **SAR 900**
- ❌ **Not within policy**: SAR 200 above the limit per room
- Total: 18 rooms × 1 night × 1,100 = **SAR 19,800**
- Above the limit: 18 × 200 = **SAR 3,600**
- The notes also say manager approval for the hotel rate is **pending**. A good answer mentions this.

</details>

---

## Step 4 · Turn it into action ✅

📋
```text
List the open issues from the offsite notes. For each one, suggest the next step. Do not assign names that are not in the notes; write "Owner to be confirmed" instead.
```

👀 **Check:** Did it invent any owners? (There are none in the notes.)

---

## Step 5 · Save a file back to Drive 💾

> ⚙️ To let Claude create files, first switch on **code execution and file creation** in Claude's settings.

📋
```text
Create a one-page offsite checklist (budget, hotel issue, open issues with next steps) and save it to my "AI-Lab-Test" folder in Google Drive.
```

👀 **Observe:** Claude should **ask for your approval** before it acts in your Drive. Read the request before you approve.
Then open Google Drive and check that the file is there.

💬 **Discuss:** Why is "ask before acting" an important safety feature? When would you **decline**?

---

## Step 6 · 🔐 Remove access (don't skip this!)

When you no longer need a connection, remove it. Do **both**:

1. **In Claude:** Customize → Connectors → Google Drive → **Disconnect**
2. **In Google:** open [myaccount.google.com/connections](https://myaccount.google.com/connections) → find **Claude** → **Delete all connections**

✅ Then ask Claude again: *"Search my Google Drive for Travel_Policy."* It should no longer be able to access it.

> 💡 Data retrieved during a chat stays with that chat. Delete the chat if you want that retrieved data removed too.

---

## 🧠 Quick quiz

**Q1.** Why did we use a test folder with fictional files?
A) It's faster  B) To limit what the AI can reach while we learn  C) Real files don't work  D) No reason

<details><summary>🔒 Answer</summary>

**B.** Give the minimum access needed, and practise safely before using real work data (only where your organization allows it).

</details>

**Q2.** You finished a project that used a connector. What should you do?
A) Leave it connected forever  B) Review permissions and disconnect if no longer needed  C) Connect more accounts  D) Share your login with colleagues

<details><summary>🔒 Answer</summary>

**B.** Review regularly and remove access you don't need.

</details>

---

> ℹ️ Other AI assistants offer similar "connected apps" features. The same safety habits apply everywhere: **minimum access → test first → approve actions → disconnect when done.**
>
> 📖 Official guide: [Use Google Workspace connectors, Claude Help Center](https://support.claude.com/en/articles/10166901-use-google-workspace-connectors)
