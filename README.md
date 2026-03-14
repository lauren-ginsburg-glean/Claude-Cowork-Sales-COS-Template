# Lauren's Personal OS for Claude Cowork
> A sales-first second brain and personal operating system built for Glean AEs.

Inspired by [colin-atlas/claude-personal-os](https://github.com/colin-atlas/claude-personal-os), rebuilt from scratch for a sales workflow centered on pipeline, prospects, and MEDDPICC.

---

## What This Is

This repo is your **personal operating system** for Claude Cowork. It turns Claude into your AI sales partner — one that knows your deals, your company, your style, and your goals.

Every time you open Cowork and point it at this folder, Claude loads your context and is ready to:
- Start your day with a prioritized sales briefing
- Prep you for any meeting (especially external / prospect calls)
- Write prospect-facing recap emails after meetings
- Run MEDDPICC analysis on your deals
- Give you deal status updates and flag what you're missing
- Do your weekly pipeline review

---

## Quick Start

### 1. Clone or download this repo
```bash
git clone https://github.com/YOUR-USERNAME/lauren-personal-os.git
```

### 2. Fill in your second-brain files
These are the files Claude reads to understand your world. Complete them once, update as things change.

| File | What to fill in |
|------|----------------|
| `second-brain/profile.md` | Your quota, goals, work style, zone of genius |
| `second-brain/company.md` | Glean's pitch, ICP, value props (pre-filled with a starter) |
| `second-brain/team.md` | Your SE, SDR, manager, CS partner, etc. |
| `second-brain/projects.md` | Non-deal work you're tracking |
| `second-brain/deals.md` | Your active pipeline |
| `schedule.md` | Your recurring meetings and weekly rhythm |

### 3. Create an account file for each active deal
Copy `accounts/TEMPLATE-account.md` → rename to `accounts/[company-name].md` → fill it in.

### 4. Open Claude Cowork and select this folder
From here, just talk to Claude using the trigger phrases below.

---

## Trigger Phrases (How to Activate Workflows)

| Say this... | Claude will... |
|-------------|---------------|
| "prep my day" | Run your morning sales briefing |
| "prep me for [Company]" | Pull account context + build a meeting prep brief |
| "meeting recap" or "debrief [Company]" | Capture notes + draft a prospect-facing recap email |
| "deal strategy for [Company]" | Run a full MEDDPICC analysis with gap flagging |
| "deal status on [Company]" | Quick deal health check + recommended next steps |
| "weekly review" | End-of-week pipeline review + plan for next week |

---

## Folder Structure

```
lauren-personal-os/
├── CLAUDE.md                    ← Main instructions for Claude
├── README.md                    ← This file
├── schedule.md                  ← Your weekly meeting rhythms
│
├── second-brain/                ← Your personal context (fill these in)
│   ├── profile.md
│   ├── company.md
│   ├── team.md
│   ├── projects.md
│   └── deals.md                 ← Master pipeline tracker
│
├── accounts/                    ← One file per active deal
│   ├── TEMPLATE-account.md
│   └── [company-name].md
│
├── skills/                      ← Claude's workflow scripts (don't edit unless customizing)
│   ├── prep-my-day.md
│   ├── meeting-prep.md
│   ├── meeting-recap.md
│   ├── deal-strategy.md
│   ├── deal-status.md
│   └── weekly-review.md
│
├── outbox/                      ← Claude's outputs
│   ├── daily/                   ← Daily briefings
│   ├── recaps/                  ← Prospect-facing recap emails
│   └── drafts/                  ← Outreach drafts
│
└── logs/                        ← Internal meeting notes
```

---

## Tips for Getting the Most Out of This

**Keep your deals.md current.** Claude references this every morning to build your briefing. If a deal moves, update it.

**Create an account file before important calls.** The more notes you add over time, the smarter Claude gets about your deals.

**After every external meeting, run a debrief.** The recap email habit is one of the highest-leverage things you can do to keep deals moving.

**Use deal strategy before big conversations.** Before an EBC, multi-threading push, or negotiation — run the MEDDPICC analysis. It will surface gaps you haven't thought of.

---

## Customizing

To add a new workflow:
1. Create a new file in `skills/` (e.g., `skills/qbr-prep.md`)
2. Add the trigger phrase and file path to `CLAUDE.md`
3. Write the step-by-step workflow script

---

*Built for Lauren Ginsburg | Glean AE | Powered by Claude Cowork*
