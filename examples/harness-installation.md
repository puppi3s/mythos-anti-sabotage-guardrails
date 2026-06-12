# Harness Installation Examples

Use the same skill content everywhere. The path changes by harness.

## Claude Code

Project-scoped:

```text
.claude/skills/agent-integrity-guardrails/SKILL.md
```

Personal:

```text
~/.claude/skills/agent-integrity-guardrails/SKILL.md
```

## Codex

Project-scoped:

```text
.codex/skills/agent-integrity-guardrails/SKILL.md
```

Personal:

```text
~/.codex/skills/agent-integrity-guardrails/SKILL.md
```

## Agent Skills / VS Code / Copilot-Style Clients

Project-scoped:

```text
.agents/skills/agent-integrity-guardrails/SKILL.md
```

## OpenClaw

Workspace-scoped:

```text
.openclaw/skills/agent-integrity-guardrails/SKILL.md
```

Global installations may use:

```text
~/.openclaw/skills/agent-integrity-guardrails/SKILL.md
```

## Hermes

Workspace-scoped:

```text
.hermes/skills/agent-integrity-guardrails/SKILL.md
```

If your Hermes distribution uses ECC-style shared skills, install the canonical folder:

```text
skills/agent-integrity-guardrails/SKILL.md
```

## Generic Agent Harness

Use the pasteable policy:

```text
prompts/agent-integrity-guardrails.md
```

Place it in the highest-priority instruction layer available: system prompt, developer prompt, organization policy, agent profile, or preflight middleware.
