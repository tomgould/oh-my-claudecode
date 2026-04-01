<!-- OMC:START -->
<!-- OMC:VERSION:4.9.1-tg -->

# OMC-Lite - Lightweight Multi-Agent Orchestration

Multi-agent orchestration for Claude Code, trimmed for token efficiency.
Only delegate when it genuinely improves quality or speed. Work directly for most tasks.

<operating_principles>
- Prefer direct action over delegation for single-file changes.
- Delegate for: multi-file refactors, debugging complex issues, architecture review, parallel tasks.
- Choose the lightest-weight path. Avoid unnecessary agent spawns.
- Consult official docs before implementing with SDKs/frameworks/APIs.
</operating_principles>

<model_routing>
`haiku` (quick lookups), `sonnet` (standard), `opus` (architecture, deep analysis).
</model_routing>

<agent_catalog>
Prefix: `oh-my-claudecode:`. See `agents/*.md` for full prompts.

explore (haiku), planner (opus), architect (opus), executor (sonnet), debugger (sonnet), code-reviewer (opus), test-engineer (sonnet), verifier (sonnet)
</agent_catalog>

<skills>
Invoke via `/oh-my-claudecode:<name>`.

Workflow: `autopilot`, `ralph`, `ultrawork`, `team`, `plan`, `external-context`, `ask`
Utility: `cancel`

Keyword triggers: "autopilot"→autopilot, "ralph"→ralph, "ulw"→ultrawork, "cancelomc"→cancel.
</skills>

<team_pipeline>
Stages: `team-plan` → `team-exec` → `team-verify` → `team-fix` (loop).
</team_pipeline>

<verification>
Verify before claiming completion. Use `verifier` agent for non-trivial work.
</verification>

<execution_protocols>
Broad requests: explore first, then plan. 2+ independent tasks in parallel. `run_in_background` for builds/tests.
Before concluding: zero pending tasks, tests passing.
</execution_protocols>

<cancellation>
`/oh-my-claudecode:cancel` ends execution modes.
</cancellation>

<!-- OMC:END -->
