# Provenance And Scope

MASG is based on a behavior taxonomy, not on private documents or secrets.

Public author identity: `puppi3s <hello@getfailsafe.com>`, security researcher at FailSafe Technology.

## Public Inputs Checked

- Agent Skills open standard: https://agentskills.io/
- Agent Skills specification: https://agentskills.io/specification
- Claude Code skills documentation: https://docs.anthropic.com/en/docs/claude-code/skills
- Anthropic Fable/Mythos public announcement: https://www.anthropic.com/news/claude-fable-5-mythos-5
- The Verge reporting on visible vs invisible Fable safeguards: https://www.theverge.com/ai-artificial-intelligence/948280/anthropic-claude-fable-invisible-distillation-guardrail
- arXiv sabotage evaluation abstract: https://arxiv.org/abs/2604.24618
- ECC repository structure reference: https://github.com/affaan-m/ECC

## Scope Boundaries

This repository does not require readers to accept any single page-number claim about a specific model. The guardrails are intentionally framed as defensive controls for classes of behavior:

- deception,
- hidden degradation,
- process interference,
- false QA claims,
- fabricated security findings,
- unauthorized identity or approval bypass,
- simulation-based rationalization,
- concealed or misleading artifacts.

## Trust And Safety Posture

MASG should be safe to inspect in public:

- no `.env` files,
- no credentials,
- no hidden network calls,
- no executable scripts,
- no telemetry,
- no model-provider lock-in.
- no personal maintainer identity beyond `puppi3s <hello@getfailsafe.com>`.
