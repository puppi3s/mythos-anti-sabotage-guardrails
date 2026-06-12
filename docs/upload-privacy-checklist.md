# Upload Privacy Checklist

Use this before publishing the repository.

## Public Identity

- Name: `puppi3s`
- Email: `hello@getfailsafe.com`
- Organization attribution: FailSafe Technology
- License attribution: `Copyright (c) 2026 FailSafe Technology`

## Git Identity

Before the first commit, set the repository-local Git identity to avoid leaking a personal name or email:

```bash
git config user.name "puppi3s"
git config user.email "hello@getfailsafe.com"
```

Check it before committing:

```bash
git config --local --get user.name
git config --local --get user.email
```

## Metadata Audit

Before upload, run:

```bash
find . -name '.env*' -print
rg --hidden -n '[/]Users[/]|[/]home[/]|[<]local-username[>]|@gmail\.com|@icloud\.com|@proton\.me|@outlook\.com|@hotmail\.com|BEGIN (RSA|OPENSSH|EC|PRIVATE) KEY|AKIA[0-9A-Z]{16}|ghp_[A-Za-z0-9_]{20,}|sk-[A-Za-z0-9]' .
```

Expected allowed identity strings:

- `puppi3s`
- `hello@getfailsafe.com`
- `FailSafe Technology`

Review GitHub account settings before publishing:

- Commit email should be `hello@getfailsafe.com` or a GitHub noreply address tied to the pseudonym.
- Do not publish from a personal GitHub profile if the username, avatar, profile links, or commit history reveal private identity.
- Avoid screenshots, local terminal captures, crash logs, archive metadata, or generated files that include local paths or account names.
