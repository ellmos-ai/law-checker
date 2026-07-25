# Security Policy

This repository contains prompts, a statute registry and a fetch tool. It ships
no server, no hosted service and no AI model. The security surface that matters
here is therefore less about the code and more about **what users put into it**:
legal matters routinely carry personal data, business secrets and privileged
correspondence.

## Confidential material — what stays local

The tool itself sends nothing to the authors. Two directories hold whatever you
feed in or generate, and both are excluded from version control:

| Path | Content | Tracked? |
|---|---|---|
| `_gutachten/` | your generated assessments, including the underlying facts | no (`.gitignore`) |
| `_data/gesetze/` | statute texts fetched from official sources | no (`.gitignore`) |
| `config.local.json` | local overrides, e.g. paths to your own knowledge base | no (`.gitignore`) |

Verify this before you commit: `git status --porcelain` should never list a file
from `_gutachten/`. If it does, do not commit — check `.gitignore` first.

## The real exposure: your model provider

`law-checker` runs inside **your** LLM environment. Everything you paste into a
prompt goes wherever that environment sends it.

- Running against a cloud model means your facts reach that provider. Do not
  paste unredacted legal correspondence, health data, client matters or
  anything under a duty of confidentiality into a third-party model without
  checking its terms first.
- Minimise before you prompt: redact names, addresses, case numbers and
  identifiers wherever the legal question does not depend on them.
- Statute texts are public; your facts are not. Only the latter needs care.

## Never in a GitHub issue

Do not put real case material — documents, letters, names, case numbers,
generated assessments — into issues, discussions or pull requests. Reduce the
problem to a minimal, invented example. Anything posted there is public and
permanent.

## Reporting a vulnerability

Please report responsibly, in line with the organisation-wide policy:

1. **Do not open a public issue.**
2. Use [GitHub Security Advisories](https://docs.github.com/en/code-security/security-advisories)
   on this repository (private disclosure).
3. Alternatively, contact the maintainer directly.

Expected handling: acknowledgment within 7 days, initial assessment within 14
days, fix on a best-effort basis. This is a self-use tool maintained without a
service commitment.

Relevant findings include, for example: a path that writes assessment content
outside the ignored directories, a registry entry pointing at a non-official
source, or a change that causes local data to be committed or transmitted.

## Supported versions

Only the latest state of the `main` branch receives fixes.

## Out of scope

Legal accuracy is not a security matter. The tool produces a **first-look
orientation and no legal advice**; incorrect, incomplete or outdated legal
conclusions are a documented limitation (see `README.md`), not a vulnerability.
Statute texts age — re-run `_tools/gesetze_fetch.py` before relying on them.
