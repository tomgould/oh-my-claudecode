<!-- Parent: ../AGENTS.md -->

# skills

8 skill directories for workflow automation.

## Purpose

Skills are reusable workflow templates invoked via `/oh-my-claudecode:skill-name`.

## Key Files

### Execution Mode Skills

| File | Skill | Purpose |
|-----------|-------|---------|
| `autopilot/SKILL.md` | autopilot | Full autonomous execution from idea to working code |
| `ultrawork/SKILL.md` | ultrawork | Maximum parallel agent execution |
| `ralph/SKILL.md` | ralph | Persistence until verified complete |
| `team/SKILL.md` | team | N coordinated agents with task claiming |

### Planning Skills

| File | Skill | Purpose |
|-----------|-------|---------|
| `plan/SKILL.md` | omc-plan | Strategic planning with interview workflow |

### Utility Skills

| File | Skill | Purpose |
|-----------|-------|---------|
| `ask/SKILL.md` | ask | Ask Claude, Codex, or Gemini via `omc ask` and capture an artifact |
| `cancel/SKILL.md` | cancel | Cancel any active OMC mode |

## Skill Categories

| Category | Skills | Trigger Keywords |
|----------|--------|------------------|
| Execution | autopilot, ultrawork, ralph, team | "autopilot", "ulw", "ralph", "team" |
| Planning | omc-plan | "plan this" |
| Utility | ask, cancel | "stop", "cancel" |

## Auto-Activation

| Skill | Auto-Trigger Condition |
|-------|----------------------|
| autopilot | "autopilot", "build me", "I want a" |
| ultrawork | "ulw", "ultrawork" |
| ralph | "ralph", "don't stop until" |
| cancel | "stop", "cancel", "abort" |
