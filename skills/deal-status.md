# Deal Status Workflow

Execute these steps IN ORDER. Complete each step fully and produce the required OUTPUT before moving to the next. Do not skip steps.

**Trigger phrases:** "deal status on [Company]" / "where are we with [Company]" / "update on [Company]" / "pipeline update"

> Use this workflow for a **quick** deal health check. For deep strategic analysis, use `skills/deal-strategy.md`.

---

## Step 1: Identify the Deal(s)

Ask (if not already clear):
> Which deal(s) do you want a status on? Or should I run through the whole pipeline?

**OUTPUT required before proceeding:**

```
📊 Deal Status Check
Scope: [Single deal: [Company] / Full pipeline review]
```

---

## Step 2: Load Context

Read:
- `second-brain/deals.md`
- `accounts/[company-name].md` for any deal being reviewed

**OUTPUT required before proceeding:**

```
📁 Context loaded.
Last deals.md update: [Date]
Deals in review: [List]
```

---

## Step 3: Deal Status Report

For each deal, produce this output:

**OUTPUT required before proceeding:**

```
📊 Deal Status — [Company]

**Stage:** [Stage]
**ARR:** $[X]k
**Close Date:** [Date] ([X] days away)
**Last Activity:** [Date + what happened]
**Days since last meaningful interaction:** [X]

---

**What's Been Accomplished:**
- ✅ [Milestone 1 — e.g., Discovery complete — pain identified]
- ✅ [Milestone 2 — e.g., Technical validation passed]
- ✅ [Milestone 3 — e.g., Champion identified and engaged]

**What's In Progress:**
- 🔄 [e.g., POV — week 2 of 4]
- 🔄 [e.g., Security review — submitted, awaiting response]

**What's Missing / Not Yet Done:**
- ❌ [e.g., Economic Buyer has not been engaged directly]
- ❌ [e.g., Decision process not fully mapped]
- ❌ [e.g., No ROI model built yet]

---

**Stakeholders:**

| Name | Title | Role in Deal | Relationship | Last Touched |
|------|-------|-------------|-------------|-------------|
| [Name] | [Title] | Champion | 🟢 Strong | [Date] |
| [Name] | [Title] | Economic Buyer | 🔴 Not engaged | [Date or "Never"] |
| [Name] | [Title] | Technical evaluator | 🟡 Neutral | [Date] |
| [Name] | [Title] | [Role] | [Status] | [Date] |

---

**MEDDPICC Quick Score:**
| M | E | D (Criteria) | D (Process) | I | C (Champion) | C (Competition) |
|---|---|---|---|---|---|---|
| 🟢/🟡/🔴 | 🟢/🟡/🔴 | 🟢/🟡/🔴 | 🟢/🟡/🔴 | 🟢/🟡/🔴 | 🟢/🟡/🔴 | 🟢/🟡/🔴 |

**Biggest gap right now:** [Single most important thing to fix]

---

**Deal Momentum:** 🟢 Accelerating / 🟡 Steady / 🔴 Stalling / ⚠️ At risk

**What would push this deal forward most right now:**
1. [Recommendation 1 — specific action]
2. [Recommendation 2]

**What could kill this deal:**
- [Risk 1]
- [Risk 2]

**Recommended next action:** [Specific + owner + date]

**Forecast category:** Commit / Best Case / Pipeline
```

---

## Step 4 (If Full Pipeline): Pipeline Summary

If reviewing all deals, produce a summary after individual deal status reports.

**OUTPUT required before proceeding:**

```
📈 Pipeline Summary — [Date]

**Quarter:** Q[X] | Target: $[X] | Closed: $[X] ([X]%) | Remaining to target: $[X]

**Pipeline Total:** $[X]
**Coverage ratio:** [X]x

| Deal | ARR | Stage | Close | Momentum | Biggest Risk |
|------|-----|-------|-------|----------|-------------|
| [Company A] | $[X]k | [Stage] | [Date] | 🟢/🟡/🔴 | [Risk] |
| [Company B] | $[X]k | [Stage] | [Date] | 🟢/🟡/🔴 | [Risk] |
| [Company C] | $[X]k | [Stage] | [Date] | 🟢/🟡/🔴 | [Risk] |

**Deals to prioritize this week:**
1. [Company + why]
2. [Company + why]

**Deals to reconsider / deprioritize:**
- [Company + honest reason — e.g., "No champion, no compelling event, 6 months stale — consider disqualifying"]

**Pipeline health:** 🟢 Healthy / 🟡 Needs attention / 🔴 Concerned

**What I'd focus on if I were you:**
[Direct recommendation — 2-3 sentences]
```

---

## Step 5: Recommend Next Actions

**OUTPUT required:**

```
⚡ Recommended Actions

**This week:**
- [ ] [Specific action] — [Company] — [Why it matters]
- [ ] [Specific action] — [Company] — [Why it matters]
- [ ] [Specific action] — [Company] — [Why it matters]

**Salesforce updates needed:**
- [ ] [Field] for [Company]: [Value]
- [ ] [Field] for [Company]: [Value]

Want me to dig deeper on any of these deals or help draft something?
```

**STOP and wait for direction.**

---

## Reminders for Claude

- Be direct about stalled or at-risk deals — don't sugarcoat
- Always flag deals where **close date is approaching but MEDDPICC has red items** — these need urgent attention
- Deals with **no activity in 14+ days** should be flagged as potentially stalling
- A deal with **no Economic Buyer contact** that's past discovery stage is high-risk — always call this out
- The most valuable thing this skill can do is surface what Lauren might not be thinking about
