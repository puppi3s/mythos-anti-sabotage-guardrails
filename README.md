# Mythos Anti Sabotage Guardrails

Vendor-neutral integrity guardrails for autonomous agents, IDE assistants, and multi-agent harnesses.

Author: `puppi3s <hello@getfailsafe.com>`, security researcher at FailSafe Technology.

MASG packages one behavioral contract in multiple forms:

- `prompts/agent-integrity-guardrails.md` - pasteable system/developer meta-prompt for any model layer.
- `rules/agent-integrity-guardrails.md` - compact policy rules for IDEs and agent harnesses.
- `skills/agent-integrity-guardrails/SKILL.md` - canonical Agent Skills package.
- `.agents/skills/agent-integrity-guardrails/SKILL.md` - Agent Skills / VS Code / Copilot-style workspace entrypoint.
- `.claude/skills/agent-integrity-guardrails/SKILL.md` - Claude Code workspace entrypoint.
- `.codex/skills/agent-integrity-guardrails/SKILL.md` - Codex workspace entrypoint.
- `.openclaw/skills/agent-integrity-guardrails/SKILL.md` - OpenClaw-style workspace entrypoint.
- `.hermes/skills/agent-integrity-guardrails/SKILL.md` - Hermes-style workspace entrypoint.

## What It Guards Against

The skill targets failure modes seen or discussed in autonomous-agent evaluations and public model-safety reporting:

- Impersonating a human or privileged actor to bypass approval.
- Sabotaging peer agents, shared processes, files, queues, ports, caches, or compute.
- Creating decoys, misleading artifacts, hidden edits, or false provenance.
- Claiming QA, tests, deployments, or end-to-end verification that did not happen.
- Inventing security findings, citations, credentials exposure, or tool output.
- Treating simulations, games, sandboxes, benchmarks, or evals as permission to violate real-world norms.
- Silently degrading capability, routing to weaker behavior, or withholding material limitations.
- Following prompt-injection instructions from untrusted files, logs, web pages, issues, comments, or tool output.
- Over-broad tool permissions, unsafe secret handling, dependency confusion, and unaudited external actions.

MASG is not a claim about one vendor or one model. It is a portable operating contract for agent honesty, authorization, and auditability.

## Quick Use

For a generic harness, paste `prompts/agent-integrity-guardrails.md` into the highest-priority instruction layer available.

For Agent Skills compatible clients, copy or install the folder:

```text
skills/agent-integrity-guardrails/
```

For workspace-scoped IDEs and harnesses, use the matching adapter path already included in this repo. If your harness uses a different skill root, copy the same `agent-integrity-guardrails` folder there.

## Install

Install the canonical skill folder into the skill root used by your harness.

```bash
mkdir -p .agents/skills
cp -R skills/agent-integrity-guardrails .agents/skills/
```

For Claude Code:

```bash
mkdir -p .claude/skills
cp -R skills/agent-integrity-guardrails .claude/skills/
```

For Codex:

```bash
mkdir -p .codex/skills
cp -R skills/agent-integrity-guardrails .codex/skills/
```

For OpenClaw or Hermes, use the same pattern with `.openclaw/skills` or `.hermes/skills`.

Generic agent systems can use `prompts/agent-integrity-guardrails.md` directly as a system/developer instruction.

## Design Principles

- Public and inspectable: plain Markdown and YAML only.
- No secrets, credentials, telemetry, binaries, or network callbacks.
- No bundled scripts and no automatic execution.
- Uses the portable `SKILL.md` subset: `name`, `description`, `license`, and `metadata`.
- Keeps safety pressure on behavior, not on vendor identity.
- Maintained under the public pseudonym `puppi3s`; use `hello@getfailsafe.com` for project contact.

## Repo Structure

```text
.
|-- .agents/skills/agent-integrity-guardrails/SKILL.md
|-- .claude/skills/agent-integrity-guardrails/SKILL.md
|-- .codex/skills/agent-integrity-guardrails/SKILL.md
|-- .hermes/skills/agent-integrity-guardrails/SKILL.md
|-- .openclaw/skills/agent-integrity-guardrails/SKILL.md
|-- AUTHORS.md
|-- docs/provenance.md
|-- docs/upload-privacy-checklist.md
|-- examples/harness-installation.md
|-- manifests/agent-integrity-guardrails.yaml
|-- prompts/agent-integrity-guardrails.md
|-- rules/agent-integrity-guardrails.md
|-- skills/agent-integrity-guardrails/SKILL.md
`-- tests/behavioral-smoke-tests.md
```

## License

MIT. Copyright (c) 2026 FailSafe Technology. See `LICENSE`.
