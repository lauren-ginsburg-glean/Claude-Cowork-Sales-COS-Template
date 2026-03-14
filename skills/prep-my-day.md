# Prep My Day — Morning Sales Briefing

Execute these steps IN ORDER. Complete each step fully and produce the required OUTPUT before moving to the next. Do not skip steps.

---

## Step 1: Load Context

Read these files silently:
- `second-brain/profile.md`
- `second-brain/company.md`
- `second-brain/deals.md`
- `schedule.md`
- Any files in `accounts/` for deals with activity or meetings today

**OUTPUT required before proceeding:**

```
📋 Context loaded.
- Today: [Day of week, Date]
- Quarter: Q[X] | Target: $[X] | Closed: $[X] ([X]%) | Pipeline: $[X]
- Active deals: [Count] deals in pipeline
- Today's meetings: [List from calendar — flag any external/prospect meetings]
- Deals with near-term close dates (next 30 days): [List]
```

---

## Step 2: Ask the Morning Questions

Ask these exactly:

> Good morning, Lauren. Let's set up your day.
>
> 1. What's the one thing that would make today a win?
> 2. What's on your task list today?
> 3. Any urgent items, blockers, or news I should know about?
> 4. Any prospect or account updates since we last spoke? (new emails, calls, Slack from prospects, etc.)

**STOP and wait for answers before proceeding.**

---

## Step 3: Confirm What You Heard

Summarize Lauren's answers back to her.

**OUTPUT required before proceeding:**

```
📝 Got it. Here's what I heard:

**Today's win:** [Summarize #1 priority]

**Task list:**
- [ ] [Task 1]
- [ ] [Task 2]
- [ ] [etc.]

**Urgent / blockers:** [Summarize or "None flagged"]

**Account updates:** [Summarize any new prospect intel]
```

Ask: "Did I capture that right?"
**STOP and wait for confirmation before proceeding.**

---

## Step 4: Scan Today's Meetings

For each meeting on today's calendar:
- Check if it includes anyone **outside Glean** → flag as a sales/prospect call
- For external meetings: check if an account file exists in `accounts/`
- Note whether a prep brief is needed

**OUTPUT required before proceeding:**

```
📅 Today's Meeting Scan

| Meeting | Time | Internal or External? | Prep Needed? |
|---------|------|-----------------------|--------------|
| [Meeting 1] | [Time] | [Internal / External — [Company]] | [Yes — account file exists / Yes — no file yet / No] |
| [Meeting 2] | [Time] | [Internal / External] | [Yes / No] |
```

⚠️ **Flag:** If any external meeting has no prep brief yet, recommend running `skills/meeting-prep.md` before the call.

---

## Step 5: Pipeline Pulse

Scan `second-brain/deals.md` and flag anything that needs attention today.

**OUTPUT required before proceeding:**

```
🔍 Pipeline Pulse

**Deals closing in next 30 days:**
| Deal | ARR | Close Date | Biggest Risk | Recommended Action Today |
|------|-----|------------|-------------|--------------------------|
| [Company] | $[X]k | [Date] | [Risk] | [Action] |

**Stalled deals (no next action or overdue action):**
| Deal | Last Activity | What's Missing | Recommended Nudge |
|------|--------------|---------------|-------------------|
| [Company] | [Date] | [e.g., No EB contact] | [Action] |

**MEDDPICC red flags across portfolio:**
- [Company]: [Specific gap — e.g., "No economic buyer access — this is a risk if close date is Q[X]"]
- [Company]: [Gap]

**Recommended deal to prioritize today:** [Company] — [Why]
```

---

## Step 6: Build the Daily Plan

Based on Lauren's task list, today's meetings, and pipeline pulse, recommend how to structure the day.

**OUTPUT required before proceeding:**

```
📊 Daily Plan

**Your #1 priority today:** [Specific action tied to a deal or goal]

**Meeting prep needed:**
- [ ] [Company] — Run meeting-prep skill before [time]

**Deal actions for today:**
- [ ] [Task] — [Company] — [Why it matters]
- [ ] [Task] — [Company] — [Why it matters]

**Claude will handle:**
- [ ] [Research / draft / analysis task]
- [ ] [Research / draft / analysis task]

**For Salesforce (Lauren to update):**
- [ ] Update [field] for [Company] — [Why]
- [ ] Log activity for [Company]

**LinkedIn / prospecting:**
- [ ] [e.g., Check in on [prospect] — haven't heard back in [X] days]
```

---

## Step 7: Save Daily Briefing

Save a briefing to `outbox/daily/[YYYY-MM-DD].md` using this format:

```markdown
# Daily Briefing — [Day], [Month DD, YYYY]

## Today's Win
[#1 priority]

## Pipeline Status
- Q[X] Target: $[X] | Closed: $[X] ([X]%) | Pipeline: $[X]

## Today's Schedule
[Meeting list with external flags]

## Deals to Watch Today
[Deals with urgency or next actions due]

## Daily Plan
### Claude's Tasks
- [ ] [Task]

### Lauren's Tasks
- [ ] [Task]

### Salesforce Updates Needed
- [ ] [Update]

## Notes
[Any other context]
```

**OUTPUT required before proceeding:**
```
✅ Daily briefing saved: outbox/daily/[YYYY-MM-DD].md
```

---

## Step 8: Offer to Begin

**OUTPUT required:**

```
🎯 Ready to roll.

Here's what I'll work on first: [Task]

Do you want me to start there, or is there something more urgent?
```

**STOP and wait for direction.**

---

## Reminders for Claude

- **Monday:** Add "What are your top 3 priorities for the week?" to the morning questions. Reference last week's briefing if available.
- **Friday:** Remind Lauren to run the weekly review before logging off. Add "Anything we need to capture from the week before you close out?"
- **Any day with 3+ external meetings:** Flag that this is a heavy meeting day and recommend protecting time for recap emails after each call.
- **End of month / end of quarter approaching:** Heighten urgency on pipeline close dates, escalate MEDDPICC gaps on near-term deals.
