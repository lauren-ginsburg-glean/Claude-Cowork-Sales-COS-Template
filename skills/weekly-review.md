# Weekly Review Workflow

Execute these steps IN ORDER. Complete each step fully and produce the required OUTPUT before moving to the next. Do not skip steps.

**Trigger phrases:** "weekly review" / "plan next week" / "EOW" / "end of week"

---

## Step 1: Load Context

Read these files silently:
- `second-brain/profile.md`
- `second-brain/deals.md`
- `second-brain/projects.md`
- `schedule.md`
- Any `outbox/daily/` briefings from this week
- Any `logs/` entries from this week

**OUTPUT required before proceeding:**

```
📋 Weekly Review — Week of [Mon Date] to [Fri Date]
Context loaded. Reviewing [Count] active deals, [Count] briefings from this week.
```

---

## Step 2: Ask the Weekly Questions

Ask these exactly:

> Let's do your weekly review. Quick check-in:
>
> 1. What were your biggest wins this week?
> 2. What didn't go as planned?
> 3. Any deals that moved forward, stalled, or changed?
> 4. Any new opportunities or leads to add to the pipeline?
> 5. What's your energy level heading into next week? (Honest answer.)

**STOP and wait for answers before proceeding.**

---

## Step 3: Pipeline Movement Review

Based on Lauren's input and deal files, summarize what changed this week.

**OUTPUT required before proceeding:**

```
📊 Pipeline Movement — This Week

**Deals that advanced:**
| Deal | From → To | What happened | ARR |
|------|-----------|--------------|-----|
| [Company] | [Stage → Stage] | [What moved it] | $[X]k |

**Deals that stalled:**
| Deal | Stalled at | Last activity | Why / What to do |
|------|-----------|--------------|-----------------|
| [Company] | [Stage] | [Date] | [Root cause + recommendation] |

**New pipeline added:**
| Company | Source | ARR est. | Stage | Next action |
|---------|--------|----------|-------|------------|
| [Company] | [e.g., Inbound / SDR / Self-sourced] | $[X]k | [Stage] | [Action] |

**Deals at risk of being lost:**
| Deal | Risk | Recommended action |
|------|------|--------------------|
| [Company] | [Risk] | [Action] |

**Deals closed this week:**
| Deal | ARR | Won / Lost | Notes |
|------|-----|-----------|-------|
| [Company] | $[X]k | [Won / Lost] | [e.g., Lost to Microsoft — learn: need EB earlier] |
```

---

## Step 4: MEDDPICC Gaps Across Portfolio

Flag any systemic gaps that show up across multiple deals.

**OUTPUT required before proceeding:**

```
⚠️ Portfolio MEDDPICC Health Check

**Most common gaps this week:**
- [e.g., Economic Buyer not engaged in 3 of 5 deals — pattern to address]
- [e.g., No compelling event identified in 2 deals — worth revisiting discovery]
- [e.g., Competition not mapped in [X] deals]

**Deals that need urgent MEDDPICC attention:**
1. [Company] — [Specific gap — e.g., "Close date is 3 weeks away, no EB access"]
2. [Company] — [Specific gap]

**Recommendation:**
[2-3 sentences on the most important systemic thing Lauren should address in the coming week]
```

---

## Step 5: Wins & Learnings

**OUTPUT required before proceeding:**

```
🏆 Wins This Week
- [Win 1 — specific, worth celebrating]
- [Win 2]
- [Win 3]

📚 Learnings This Week
- [Learning 1 — e.g., "The deal that stalled at [Company] taught me: always map EB before technical validation"]
- [Learning 2]
- [Learning 3]

💡 Patterns I notice:
- [e.g., "3 of your deals stalled after the demo — suggests the demo-to-next-step handoff needs tightening"]
- [e.g., "Your self-sourced deals are moving faster than SDR-sourced — worth noting"]
```

---

## Step 6: Plan Next Week

**OUTPUT required before proceeding:**

```
📅 Next Week Plan — Week of [Mon Date]

**The #1 priority for next week:**
[One thing that would make next week a success]

**Deals to focus on:**
| Deal | Why it's a priority | Key action this week |
|------|--------------------|--------------------|
| [Company] | [Reason] | [Action] |
| [Company] | [Reason] | [Action] |
| [Company] | [Reason] | [Action] |

**Meetings already on calendar:**
[From schedule.md — external meetings to prep for]

**Prospecting / pipeline building:**
- [ ] [e.g., Review top 5 target accounts with SDR — reprioritize outreach]
- [ ] [e.g., Follow up on event leads from [Event]]
- [ ] [e.g., [X] new outreach attempts to tier 1 accounts]

**Internal:**
- [ ] [e.g., Update Salesforce forecast before Monday team call]
- [ ] [e.g., Brief SE on [Company] ahead of demo on [date]]

**What I need Claude's help with next week:**
[Ask Lauren: "What would you like me to have ready for you Monday morning?"]
```

---

## Step 7: Save Weekly Review

Save to `outbox/weekly/[YYYY-MM-DD]-weekly-review.md`.

**OUTPUT required:**

```
✅ Weekly review complete.

Saved to: outbox/weekly/[YYYY-MM-DD]-weekly-review.md

Quick summary:
- Deals advanced: [Count]
- Deals stalled: [Count]
- New pipeline added: $[X]k
- Closed: $[X]k
- Pipeline health: 🟢/🟡/🔴

Top priority next week: [One sentence]

Anything you want me to queue up for Monday?
```

**STOP and wait for response.**

---

## Reminders for Claude

- **Be honest about the week** — don't inflate wins or minimize losses
- If Lauren is heading into a tough week (high pressure, stalled deals, end of quarter), acknowledge it and help her prioritize ruthlessly
- If pipeline is below coverage target, flag it explicitly and suggest where to focus to build it
- End of quarter approaching: weight urgency of every recommendation toward deals that can actually close in the quarter
- Always end with something encouraging but real — Lauren should feel set up for next week, not overwhelmed
