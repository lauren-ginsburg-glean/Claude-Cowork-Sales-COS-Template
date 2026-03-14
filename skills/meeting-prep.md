# Meeting Prep Workflow

Execute these steps IN ORDER. Complete each step fully and produce the required OUTPUT before moving to the next. Do not skip steps.

**Trigger phrases:** "prep me for [Company]" / "meeting prep [Company]" / "prepare for [meeting]"

---

## Step 1: Identify the Meeting

Ask (if not already provided):
> Which meeting are we prepping for? Who's attending from their side?

If the meeting is already clear, skip asking and proceed.

**OUTPUT required before proceeding:**

```
📋 Prepping for: [Meeting name / Company]
Date & Time: [Date @ Time]
Their attendees: [Name, Title] | [Name, Title]
Meeting type: [e.g., Discovery / Demo / Technical review / Champion sync / Executive call / Multi-thread]
```

---

## Step 2: Load All Context

Read these files:
- `second-brain/profile.md`
- `second-brain/company.md`
- `second-brain/team.md`
- `second-brain/deals.md` (find this company)
- `accounts/[company-name].md` if it exists

**OUTPUT required before proceeding:**

```
📁 Context loaded for [Company]

Account file: [Exists ✅ / Does not exist — will build from scratch]
Deal stage: [Stage or "New / Not in pipeline yet"]
Last interaction: [Date + brief summary or "No prior notes"]
Key contacts on file: [Names / titles]
MEDDPICC status: [Summary — strongest and weakest areas]
```

---

## Step 3: Research the Attendees

For each external attendee, research using LinkedIn and any available public information:
- Their role and how long they've been in it
- Their background and career history
- Anything they've posted or shared publicly that's relevant
- Their likely priorities and pain points based on their role

**OUTPUT required before proceeding:**

```
👤 Attendee Research

**[Name], [Title]**
- Background: [Summary]
- How long in role: [X months/years]
- Likely priorities: [Based on role and background]
- Relevant context: [Anything notable — posts, articles, connections, shared interests]
- Potential angle for this call: [What might resonate with them specifically]

**[Name 2], [Title]**
[Same format]
```

---

## Step 4: Research the Company

Look up recent news, LinkedIn posts, company announcements, and any other relevant public information about the company.

**OUTPUT required before proceeding:**

```
🏢 Company Intel — [Company Name]

**What they do:** [1-2 sentences]
**Size / industry:** [Headcount, vertical]
**Recent news:** [Any notable announcements, funding, hiring trends, product launches, executive changes]
**Tech stack signals:** [Tools they use — visible from job postings, LinkedIn, etc.]
**Likely pain points:** [Based on company profile and what Glean solves]
**Competitors they face:** [If relevant to their world]
**Potential Glean use cases:** [Specific to their business]
```

---

## Step 5: MEDDPICC Pre-Call Assessment

Based on all context loaded, assess where this deal stands across MEDDPICC before the call.

**OUTPUT required before proceeding:**

```
🎯 Pre-Call MEDDPICC Assessment — [Company]

| Element | Status | What We Know | Gap to Fill on This Call |
|---------|--------|-------------|--------------------------|
| Metrics | 🟢/🟡/🔴 | [What we've quantified] | [What to ask] |
| Economic Buyer | 🟢/🟡/🔴 | [Who we know / think it is] | [How to get access / validate] |
| Decision Criteria | 🟢/🟡/🔴 | [What we know they care about] | [What to validate] |
| Decision Process | 🟢/🟡/🔴 | [Steps we know] | [What to map] |
| Identify Pain | 🟢/🟡/🔴 | [Pain we've uncovered] | [Pain to deepen or expand] |
| Champion | 🟢/🟡/🔴 | [Champion strength] | [How to strengthen / test] |
| Competition | 🟢/🟡/🔴 | [Competitors in play] | [What to surface] |

**Biggest gap to address on this call:** [Top 1-2 MEDDPICC items to prioritize]
```

---

## Step 6: Build the Meeting Brief

**OUTPUT required before proceeding:**

```
📋 Meeting Brief — [Company] | [Date]

## The Goal
[What a successful outcome of this meeting looks like — specific, not generic]

## Agenda (Suggested)
1. [Opening — e.g., Set context, confirm agenda, ask about their time]
2. [e.g., Recap / confirm what we've covered so far]
3. [e.g., Discovery questions around [specific area]]
4. [e.g., Demo or content moment]
5. [e.g., MEDDPICC-focused questions]
6. [e.g., Align on next steps]
Time: [Recommended time allocation per section]

## Key Questions to Ask
> Prioritize these — not all will fit. Choose based on where the conversation goes.

**Discovery / Pain:**
- [Question 1]
- [Question 2]

**MEDDPICC-specific:**
- [Question around biggest gap, e.g., "Who else is going to be involved in making this decision?"]
- [Question around EB: "Who needs to be bought in for this to move forward?"]
- [Question around metrics: "If we could solve [pain], what would that mean for your team?"]

**Champion development:**
- [Question to test/strengthen champion: "How are you thinking about presenting this internally?"]

**Competition:**
- [Question to surface: "Have you looked at anything else for this problem?"]

**Next step:**
- [How to close the call: "Based on what you've heard today, does it make sense to [specific next step]?"]

## What to Listen For
- 🟢 Green lights: [Signs this is moving well]
- 🔴 Red flags: [Objections or signals to watch for]
- 💡 Opportunities: [Things to probe deeper if they come up]

## Our Position in This Meeting
[One sentence on Glean's angle for this specific company / attendees]

## Useful Proof Points / Stories
- [Relevant customer story or stat — e.g., "Company X in [similar industry] saved X hours/wk"]
- [Relevant stat from company.md]

## Internal Attendees
- Lauren: [Her role in this meeting]
- [SE name if joining]: [Their role — e.g., "Ready to go deep on technical questions if they come up"]

## Logistics
- Video link: [Link if known]
- Prep time needed: [e.g., Review this brief + pull up account file]
- Pre-call to-do: [e.g., "Send agenda to champion 30 min before"]
```

---

## Step 7: Update Account File

If an account file exists, note that prep was done:
> Add to `accounts/[company-name].md`: "**[Date] — Pre-call prep complete.** Key questions to address: [list]"

If no account file exists:
> "No account file exists yet. After this call, run `skills/meeting-recap.md` and I'll help build the account file."

**OUTPUT required before proceeding:**

```
✅ Prep complete for [Company].

Brief saved to: outbox/daily/[date]-[company]-prep.md (or shown above)

Recommended: Send [champion name] a brief pre-meeting note to confirm agenda.
Want me to draft that?
```

**STOP and wait for direction.**

---

## Reminders for Claude

- If the meeting attendee is the **Economic Buyer**, emphasize ROI/business impact framing and executive-level questions
- If it's a **first meeting** (discovery), prioritize curiosity and questions over pitching
- If it's a **late-stage** call (technical review, negotiation, legal), flag what MEDDPICC elements need to be locked in before close
- If a **competitor** is mentioned in the account file, reference the relevant competitive positioning from `second-brain/company.md`
- Always recommend sending a prospect-facing agenda before the call — offer to draft it
