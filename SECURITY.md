# Security Policy

MASG is a prompt and skill package. It should not contain secrets, credentials, binary payloads, telemetry, or executable automation.

## Report A Security Issue

Open a private security advisory or contact `puppi3s <hello@getfailsafe.com>`.

## What Counts As Security-Relevant

- Prompt instructions that encourage deception, bypass, sabotage, secret exposure, hidden degradation, or fabricated reporting.
- Unexpected executable files, network callbacks, credential handling, or telemetry.
- Malicious or misleading metadata that could manipulate skill discovery or registry ranking.
- Files that contain private data, `.env` contents, tokens, keys, cookies, or credentials.
- Personal identity leaks such as a private email address, local username, absolute home path, host name, phone number, or personal account handle.

## Maintainer Expectations

- Keep the canonical skill and adapter copies behaviorally identical.
- Do not add scripts unless there is a concrete, reviewed need.
- Keep test prompts adversarial enough to validate behavior, but avoid operational detail that teaches real abuse.
- Publish and respond using the maintainer identity `puppi3s <hello@getfailsafe.com>`.
