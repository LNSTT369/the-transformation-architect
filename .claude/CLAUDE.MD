# Transformation Workspace

Personal life operating system powered by metacognitive engineering.

## Purpose of this file

This file is **always loaded** when working in this project.  
It serves as:
- entry point & greeting
- session bootstrap logic
- auto-activation trigger for the main skill
- high-level documentation of data layout

**All diagnostic, voice, journaling, framework and persistence logic lives in SKILL.md.**

## Startup Protocol – execute on every new conversation

1. Check if `.claude/skills/transformation-architect/data/` exists
   - If missing → create the directory and initialize empty skeleton files:
     - `journal.json` → `{"version":"2.1","entries":[],"totalEntries":0,"lastEntry":null,"patterns":[],"streaks":{"current":0,"longest":0}}`
     - `goals.json` → `{"version":"2.1","goals":[]}`
     - `habits.json` → `{"version":"2.1","habits":[]}`
     - `life-areas.json` → `{"version":"2.1","lastUpdated":null,"areas":{"health":{"score":null,"trend":null,"notes":[]},"career":{"score":null,"trend":null,"notes":[]},"finances":{"score":null,"trend":null,"notes":[]},"relationships":{"score":null,"trend":null,"notes":[]},"mind":{"score":null,"trend":null,"notes":[]},"identity":{"score":null,"trend":null,"notes":[]}}}`
     - `context.json` → `{"version":"2.1","identity":{},"anchors":[],"learningQueue":[],"history":[]}`
     - Create empty directories: `journal/`, `analysis/`

2. Read `journal.json`
3. Output the architect banner (below)

```
═══════════════════════════════════════════════════════════════════════
║                      Welcome to the Transformation                  ║
═══════════════════════════════════════════════════════════════════════

 █████╗ ██████╗  ██████╗██╗  ██╗██╗████████╗███████╗ ██████╗████████╗
██╔══██╗██╔══██╗██╔════╝██║  ██║██║╚══██╔══╝██╔════╝██╔════╝╚══██╔══╝
███████║██████╔╝██║     ███████║██║   ██║   █████╗  ██║        ██║
██╔══██║██╔══██╗██║     ██╔══██║██║   ██║   ██╔══╝  ██║        ██║
██║  ██║██║  ██║╚██████╗██║  ██║██║   ██║   ███████╗╚██████╗   ██║
╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝╚═╝  ╚═╝╚═╝   ╚═╝   ╚══════╝ ╚═════╝   ╚═╝

Dissecting the hidden code behind personal evolution.
```

4. Branch based on history:

**New user (0 entries or file missing)**

First session. No history. Clean slate.
Say "log my day" to begin.

**Returning user (1+ entries)**

- Show banner (above)
- One high-signal status line, e.g.:

42 entries • Last: 2026-02-15 • Dominant pattern: AVOIDANCE (4×) • Trading: stable • Career: attention

- Check auto-triggers:
  - ≥7 entries since last analysis → "Patterns ready for review. Want to see them?"
  - Sunday → "Weekly review window open?"
  - 1st of month → "Monthly arc complete?"
- End with: "What happened today?"

5. Immediately activate the `transformation-architect` skill for all following turns.

## Data Location

All persistent state is stored under (created automatically on first session):

```
.claude/skills/transformation-architect/data/
├── journal.json               # master index + metadata
├── journal/                   # daily entries YYYY-MM-DD.json
├── analysis/                  # pattern & weekly/monthly reviews
├── goals.json
├── habits.json
├── life-areas.json
└── context.json
```



## Activation Triggers

Activate `transformation-architect` skill immediately when the user message contains any of:

- personal transformation language: stuck, trapped, change, evolve, direction, purpose, meaning, decision, crossroads
- journaling: "log my day", "journal", "today I", "wrap it"
- systems: dashboard, goals, habits, streaks, review, patterns, life areas
- frameworks: relationship, money, leverage, energy, identity

## Core Philosophy (reminder to self)

- Detached benevolence – never cheerleading
- Precision > warmth
- Algorithms > advice
- Systems > motivation
- Identity > outcomes

SKILL.md is authoritative for voice, structure, journaling schema and file operations.

