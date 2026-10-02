# Contributing to DataLife Mobile App

Thank you for helping build a patient-sovereign mobile client. The organization-wide
[contribution rules](https://github.com/datalife-ehealth/.github/blob/main/CONTRIBUTING.md)
apply here; this file adds mobile privacy and platform expectations.

## Before coding

1. Search existing issues and pull requests.
2. Comment on or claim a focused issue before significant implementation work.
3. Use an RFC for framework changes, vault or key lifecycle changes, recovery,
   identity mapping, new network destinations, or new clinical workflows.
4. Use invented identifiers and records in every fixture, screenshot, recording,
   issue, and demo.

## Definition of done

A mobile change should include tests appropriate to its risk:

- unit tests for serialization, redaction, and state transitions;
- contract tests for core integrations;
- keyboard, screen-reader, text scaling, contrast, and reduced-motion checks;
- Android and iOS behavior where a platform security boundary is involved;
- evidence that PII and grants stay out of logs, URLs, analytics, notifications,
  backups, clipboard, screenshots, and background previews as applicable; and
- documentation for failure, recovery, migration, and device-loss behavior.

Do not submit real patient data, credentials, signing material, generated builds, or
sensitive screenshots. Never weaken server authorization or the Zero Cloud PII
Invariant to make a workflow pass.

## Pull requests

Keep one concern per pull request, link its issue or RFC, and complete the privacy,
platform, and test sections in the template. Approval from the repository steward is
required. Use `feat/`, `fix/`, or `docs/` branches from `main`.
