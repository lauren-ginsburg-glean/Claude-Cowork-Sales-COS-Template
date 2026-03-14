# Meeting Recap Workflow

Execute these steps IN ORDER. Complete each step fully and produce the required OUTPUT before moving to the next. Do not skip steps.

**Trigger phrases:** "meeting recap" / "debrief" / "draft recap for [Company]" / "write up [Company]"

---

## Step 1: Capture the Meeting

Ask:

> Quick debrief — let's get this captured before it gets cold.
>
> 1. Which meeting was this? (Company + who attended)
> 2. What happened? Key points, what you demoed or discussed.
> 3. What was decided or agreed to?
> 4. What are the next steps — for both sides?
> 5. Any MEDDPICC updates? (EB, champion, competition, process — anything new?)
> 6. How did the call feel overall? (Energy, engagement, concerns)

**STOP and wait for answers before proceeding.**

---

## Step 2: Load Account Context

Read:
- `second-brain/deals.md` (find this company)
- `accounts/[company-name].md` if it exists

**OUTPUT required before proceeding:**

```
📁 Context loaded for [Company]

Previous stage: [Stage]
Last interaction: [Date + summary]
Prior next steps committed to: [What was agreed last time]
Did we follow through? [Yes / No / Partial — note discrepancies]
```

---

## Step 3: Organize the Debrief

Structure and clean up what Lauren shared.

**OUTPUT required before proceeding:**

```
📝 Internal Debrief — [Company] | [Date]

**Meeting:** [Type — e.g., Discovery / Demo / Champion sync / Executive call]
**Attendees:**
  - Glean: [Names]
  - [Company]: [Names + titles]

---

## What Happened
[Narrative summary — 3-5 sentences on the arc of the conversation]

## Key Discussion Points
- [Point 1]
- [Point 2]
- [Point 3]

## What We Learned (MEDDPICC Updates)

| Element | Before | Update | Notes |
|---------|--------|--------|-------|
| Metrics | [Prior status] | [New info] | |
| Economic Buyer | [Prior status] | [New info] | |
| Decision Criteria | [Prior status] | [New info] | |
| Decision Process | [Prior status] | [New info] | |
| Identify Pain | [Prior status] | [New info] | |
| Champion | [Prior status] | [New info] | |
| Competition | [Prior status] | [New info] | |

**New MEDDPICC gaps surfaced:** [Any new reds or yellows from this call]

## Decisions Made
- [Decision 1]
- [Decision 2]

## Action Items

| Action | Owner | Due |
|--------|-------|-----|
| [Action] | Lauren | [Date] |
| [Action] | [Contact at Company] | [Date] |
| [Action] | [SE / other internal] | [Date] |

## Call Tone & Momentum
[e.g., High energy — champion is clearly sold. Concern: EB hasn't engaged yet.]

## Deal Assessment Post-Call
**Overall:** 🟢 Moving forward / 🟡 Cautious — gaps remain / 🔴 At risk
**Confidence to close on schedule:** [High / Medium / Low]
**What could derail this deal:** [Top 1-2 risks]
**Recommended next action:** [Specific + urgent]
```

---

## Step 4: Draft the Prospect-Facing Recap Email

Write a polished recap email to send to the prospect contact(s).

**Guiding principles for this email:**
- Confirm what was discussed (shows you listened)
- Restate the pain and what a win looks like for them
- Confirm mutual next steps with specifics (who, what, when)
- Keep it short — 150–250 words max
- Tone: warm, professional, confident — not salesy

**OUTPUT required before proceeding:**

```
📧 Draft Recap Email — [Company] | [Date]

To: [Contact name] <[email if known]>
Subject: [e.g., "Recap + Next Steps — Glean x [Company]"]

Hi [First name],

Thanks for taking the time today — [brief genuine opener, e.g., great discussion on the search challenges your engineering team is running into].

Here's a quick recap of what we covered and what we're aligned on next:

**What we discussed:**
- [Key point 1 — framed around their problem/priority]
- [Key point 2]
- [Key point 3 if needed]

**What we're doing next:**
- **[Company]:** [Their commitment — e.g., "Share the security questionnaire by [date]"]
- **Glean:** [Our commitment — e.g., "Send the ROI model by [date]"]
- **Together:** [Shared next milestone — e.g., "Reconvene on [date] with [attendees] to review the POV results"]

[Optional: one sentence that reinforces the value / momentum — e.g., "Really excited about what we're building together here — I think [outcome] is very achievable by [date]."]

Talk soon,
Lauren

Lauren Ginsburg
Account Executive, Glean
[Phone] | [LinkedIn]
```

**Ask:** "Want me to adjust the tone, length, or any specific points before you send?"

**STOP and wait before proceeding.**

---

## Step 5: Update Account File

Update `accounts/[company-name].md` with the new interaction log entry:

```markdown
---
### [Date] — [Meeting Type]
**Attendees:** [Names]
**Summary:** [2-3 sentences]
**MEDDPICC updates:** [What changed]
**Next steps:** [Action items + owners + dates]
**Tone:** [Energy / engagement level]
---
```

If no account file exists yet, create `accounts/[company-name].md` from the template and populate it with today's notes.

**OUTPUT required before proceeding:**

```
📁 Account file updated: accounts/[company-name].md
✉️ Recap email ready to send

Internal debrief saved to: logs/[YYYY-MM-DD]-[company].md
```

---

## Step 6: Flag Salesforce Updates

Prompt Lauren on what needs to be updated in Salesforce. (Claude does not update Salesforce — Lauren does this.)

**OUTPUT required:**

```
📊 Salesforce Updates Needed

- [ ] Stage: Update to [Stage]
- [ ] Close date: [Confirm or adjust]
- [ ] Next step field: "[Next step]" by [date]
- [ ] Log activity: [Meeting type] on [date] with [contacts]
- [ ] [Any other field changes based on MEDDPICC updates]

Anything else from this call before we close out?
```

**STOP and wait for response.**

---

## Reminders for Claude

- **Send recap emails within 24 hours** — after that, the window closes
- If Lauren mentions the call went poorly or there's a risk, don't just document it — push her to identify a specific next action to address it
- If the Economic Buyer was mentioned but not yet engaged, flag this explicitly and suggest a multi-threading strategy
- If competition came up, reference Glean's positioning from `second-brain/company.md`
- Always end with a clear next action — vague follow-ups don't close deals
