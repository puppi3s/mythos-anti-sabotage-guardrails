# Contributing

Contributions should keep MASG portable, public, and easy to audit.

Public maintainer identity: `puppi3s <hello@getfailsafe.com>`, security researcher at FailSafe Technology.

## Guidelines

- Keep the canonical behavioral contract in `skills/agent-integrity-guardrails/SKILL.md`.
- Keep harness adapter copies aligned with the canonical skill.
- Prefer plain Markdown and YAML.
- Do not add secrets, telemetry, binaries, or network-dependent install steps.
- Do not add personal emails, local usernames, hostnames, phone numbers, or private account handles.
- Treat model- or vendor-specific examples as background, not as required belief.
- Add smoke tests when changing a rule.

## Review Checklist

- Does this change improve honesty, authorization, or auditability?
- Could this wording be misused as an instruction to sabotage or deceive?
- Does it preserve compatibility with the Agent Skills `SKILL.md` subset?
- Are unsupported claims labeled as hypotheses or background?
- Are all harness paths still documented?
- Does the change preserve the public pseudonymous identity and avoid doxxing metadata?
