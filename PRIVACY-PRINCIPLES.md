# Privacy Principles

These principles describe the intended privacy posture for projects maintained by **0xterricola**.

Individual repositories should document their actual behavior where privacy-relevant functionality exists.

## Data minimization

Projects should avoid collecting, transmitting, or retaining information that is not required for their intended functionality.

Where practical, computation should remain local to the user's device or infrastructure.

## Secrets

Private keys, seed phrases, passwords, authentication tokens, API keys, recovery material, and equivalent secrets should never be intentionally logged, committed, included in telemetry, or submitted in public bug reports.

Users and contributors should treat logs and diagnostic output as potentially sensitive until reviewed.

## Network metadata

Even software that does not collect application-level personal information may expose metadata through network activity.

Depending on the project, this can include:

- IP addresses;
- node addresses;
- peer information;
- RPC endpoints;
- timing information;
- wallet addresses;
- transaction identifiers;
- public keys;
- device identifiers;
- request metadata.

Projects involving networking should document relevant exposure where known.

## Telemetry

Telemetry or analytics, if introduced, should be documented clearly.

Documentation should identify:

- what is collected;
- why it is collected;
- where it is transmitted;
- how long it is retained, if known;
- whether it can be disabled.

Absence of such documentation should not be interpreted as a universal guarantee that no third-party dependency or external service observes network activity.

## Third-party services

Projects may rely on external services such as RPC providers, APIs, package registries, relays, explorers, hosting providers, or other infrastructure.

Those services may have their own logging and privacy behavior outside the control of the project.

Relevant dependencies should be disclosed where they materially affect privacy assumptions.

## Read-only software

A tool being read-only does not mean it is privacy-neutral.

Read-only applications may still observe or expose node state, addresses, peer information, logs, identifiers, or network metadata.

Project documentation should distinguish read access from data collection, storage, and transmission.

## Project-specific disclosures

Privacy-sensitive repositories should provide a repository-specific `PRIVACY.md` or equivalent documentation when the general principles here are insufficient.

Project-specific documentation takes precedence over this document.
