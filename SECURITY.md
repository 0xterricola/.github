# Security Policy

This is the default security policy for open-source repositories maintained by **0xterricola**.

A repository-specific `SECURITY.md`, threat model, security review, or other security documentation may provide additional or overriding guidance.

## Reporting a vulnerability

Please report suspected vulnerabilities privately whenever possible.

If GitHub Private Vulnerability Reporting is enabled for the affected repository, use:

**Security → Report a vulnerability**

Do not publish exploit details, private keys, seed phrases, credentials, authentication tokens, sensitive logs, or other secrets in a public issue.

If private vulnerability reporting is unavailable, open a minimal public issue requesting a private security contact without including exploit details.

A useful report includes:

- affected repository, component, commit, or version;
- security property believed to be violated;
- reproduction steps or proof of concept;
- expected and observed behavior;
- potential impact;
- relevant environment or configuration;
- suggested mitigation, if known.

## Project maturity

Repositories may contain experimental, unfinished, research-oriented, or security-sensitive software.

Unless explicitly documented otherwise, software maintained by 0xterricola:

- has not undergone a formal independent security audit;
- should not be assumed to be vulnerability-free;
- may change substantially during development;
- may contain implementation mistakes, incomplete threat modeling, or incorrect assumptions.

Statements such as "tested", "reviewed", or "implements" describe specific work performed. They should not be interpreted as guarantees of security.

## Cryptographic software

Cryptographic implementations receive additional scrutiny because small implementation errors can have severe consequences.

Projects should prefer established standards and established cryptographic primitives rather than inventing new cryptographic constructions.

Testing against standards, reference implementations, vectors, interoperability tests, and regression tests is encouraged where applicable.

A successful test does not establish the absence of vulnerabilities.

## Wallets and blockchain software

Where applicable, project documentation should make clear:

- whether software is custodial or non-custodial;
- whether private keys or signing material are accessible to the software;
- whether transactions can be created, modified, signed, or broadcast;
- which external RPC endpoints, APIs, relays, or services are trusted;
- what network or metadata exposure may occur;
- whether functionality is read-only;
- which security assumptions users are expected to make.

## Good-faith security research

Good-faith testing and responsible vulnerability reporting are welcome.

Testing should be performed only against systems, accounts, devices, data, or infrastructure that the researcher owns or is authorized to test.

Security research should avoid unnecessary disruption, privacy violations, theft, destruction of data, unauthorized access to third-party assets, or public disclosure of exploitable details before maintainers have had a reasonable opportunity to investigate.

## Security review records

Security-sensitive repositories may maintain documents such as:

- `SECURITY_REVIEW.md`
- `THREAT_MODEL.md`
- `LIMITATIONS.md`
- `PRIVACY.md`

These documents are intended to make known assumptions, findings, unresolved risks, mitigations, and test coverage visible.

Their existence does not imply that a formal security audit has occurred.

## AI-assisted development

AI tools are used extensively in some 0xterricola projects.

AI assistance is not considered an independent security review or security audit.

See [AI-ASSISTED-DEVELOPMENT.md](AI-ASSISTED-DEVELOPMENT.md).

## No security guarantee

Security is an ongoing engineering process.

The presence of this policy, security testing, code review, threat modeling, or vulnerability remediation should not be interpreted as a guarantee that software is secure or appropriate for any particular use.
