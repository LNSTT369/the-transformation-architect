# The Transformation Architect

Metacognitive operating system for irreversible personal evolution.

A private Claude-powered life architecture that turns vague feelings of being "stuck" into precise diagnostic algorithms, identity-level rewrites, daily non-negotiables, persistent journaling, habit & goal tracking, life-area dashboards, pattern analysis, and long-term arc reviews — all without cheerleading or empty motivation.

## Core Philosophy

- Identity > outcomes  
- Systems > goals  
- Algorithms > advice  
- Precision > warmth  
- Detached benevolence, never permission-granting or validation-seeking

You are not here to feel better today.  
You are here to become someone who no longer needs to ask what to do.

## Quick Start (Recommended – 2 minutes)

1. Open a fresh terminal  
   (on Mac: Terminal.app, on Windows: PowerShell / Git Bash / Command Prompt)

2. Go to your Desktop and clone the repo into a folder named `transformation-architect`:

   ```bash
   cd ~/Desktop
   git clone https://github.com/LNSTT369/the-transformation-architect.git transformation-architect
   ```

3. Open the folder and launch Claude Code:

   ```bash
   cd transformation-architect
   claude
   ```

4. The system auto-activates. Say **"log my day"** to begin.

## How It Works

Two tightly coordinated Markdown files drive the entire experience:

| File              | Loaded when                  | Purpose                                                                 | Token footprint |
|-------------------|------------------------------|-------------------------------------------------------------------------|-----------------|
| `CLAUDE.md`       | Always (project root)        | Workspace constitution · session bootstrap · greeting · auto-activation | ~600–700 tokens |
| `SKILL.md`        | On-demand (skill match)      | Full diagnostic framework · voice rules · journaling logic · persistence | loaded lazily   |

- `CLAUDE.md` → lightweight gatekeeper that greets you, shows status, and immediately invokes the main skill  
- `SKILL.md` → the actual Transformation Architect: diagnostic structure, three-journey paths, source-code habits, journaling engine, life systems

## Key Features

- **Daily Journaling**  
  Natural-language reflection → structured diagnostic → incremental refinement → file persistence on "wrap it"

- **Identity-first diagnostics**  
  Trap · Cost · Assumption  
  Current Self → Necessary Self → The Gap  
  Three Journeys (Safe / Direct / Accelerated) + Source Code (habits · fear · internal metric)

- **Persistent Systems**  
  - Life Areas Dashboard (Trading · Career · Health · Expression · Relationships · Finances · Learning)  
  - Goals (outcome / process / identity)  
  - Habit streaks & recovery protocol  
  - Personal context layer (identity anchors, origin story, key people, dates)  
  - Learning queue & mastery tracking

- **Pattern & Review Engine**  
  Blocker pattern detection (Avoidance, Overthinking, External Locus, Permission Seeking, etc.)  
  Auto-triggered analysis after 7+ entries  
  Weekly / monthly arc synthesis

- **Framework Modules** (activate on topic)  
  - Relationship audit (5 Chimps, Energy Exchange, Tribal Roles, Boundaries)  
  - Wealth / leverage (4 Levers, Asset vs Liability, Specific Knowledge)  
  - Energy & state management

## How to Use

| What you want                        | Say / ask something like                                 |
|--------------------------------------|-----------------------------------------------------------|
| Start daily reflection               | "log my day"                                              |
| Continue reflection                  | "Also I realized…" / "One more thing…"                    |
| Finish & save entry                  | "wrap it"                                                 |
| See current life status              | "show my dashboard" / "life status"                       |
| Check goals / habits / streaks       | "my goals" / "streak check" / "habits"                    |
| Update status                        | "update trading: thriving" / "log workout"                |
| Request pattern review               | "analyze my patterns"                                     |
| Weekly / monthly arc                 | "weekly review" / "monthly review"                        |
| Relationship or money question       | "what should I do about [person/money situation]?"        |
| General life stuck / decision        | "I feel stuck" / "help me think through this" / "what should I do with my life" |

All commands are natural-language detected — no rigid syntax required.

## Directory Structure (inside project)

```
.claude/
├── CLAUDE.md                          ← always-loaded bootstrap
└── skills/
    ├── SKILL.md                       ← main architect logic
    └── transformation-architect/
        └── data/                      ← created on first use (gitignored)
            ├── journal.json
            ├── journal/
            ├── analysis/
            ├── goals.json
            ├── habits.json
            ├── life-areas.json
            └── context.json
```

## Setup & Maintenance

1. Place `CLAUDE.md` in the project root (or any parent directory Claude Code indexes)
2. Place `SKILL.md` in `.claude/skills/transformation-architect/`
3. Create the `data/` subfolder (Claude will populate files automatically)
4. Start a new conversation in the workspace → system auto-initializes

**Reset / archive**  
Delete or move `data/` folder contents when starting a clean epoch.

**Backup**  
Periodically copy the entire `data/` folder — it contains your entire evolution history.

## Principles Reminder (enforced by the system)

- No cheerleading  
- No paragraphs  
- One sentence per line when diagnosing  
- Vertical space is signal  
- Constraints liberate  
- Easy choices, hard life. Hard choices, easy life.

Your evolution is not a mystery.  
It's an algorithm waiting to be executed.