# Security Principles

These principles describe the intended security engineering posture for projects maintained by **0xterricola**.

They are engineering goals and practices, not guarantees.

## Good-faith development

Projects are developed with the intent to create useful, lawful, and technically sound software.

Security-relevant behavior should be made explicit rather than hidden behind assumptions.

Known material risks should be documented when they are identified.

## Minimize trust

Where practical, designs should minimize:

- custody of user assets;
- access to private keys or signing material;
- privileged infrastructure;
- unnecessary network services;
- unnecessary permissions;
- collection of user data;
- dependence on trusted intermediaries.

Read-only and local-first designs are preferred where they satisfy the project's goals.

## Prefer established cryptography

Projects should prefer standardized, publicly documented, and widely reviewed cryptographic primitives and protocols.

Custom cryptographic constructions should be avoided unless there is a clear research justification and their experimental nature is explicitly documented.

Protocol compatibility does not itself prove implementation security.

## Explicit threat models

Security-sensitive projects should identify relevant trust boundaries and attack surfaces.

Examples include:

- private-key handling;
- signing operations;
- QR or transport protocols;
- RPC interfaces;
- local storage;
- network metadata;
- authentication;
- serialization and parsing;
- external services;
- dependency compromise;
- hardware boundaries;
- malicious or malformed inputs.

Threat models should evolve as implementations evolve.

## Test security properties

Where feasible, security-relevant assumptions should become executable tests.

Useful techniques include:

- regression tests;
- known-answer vectors;
- interoperability tests;
- malformed-input tests;
- boundary testing;
- negative tests;
- fuzzing;
- static analysis;
- sanitizer builds;
- manual review.

Passing tests establishes only what those tests exercised.

## Track findings

Security findings should be recorded with enough context to understand their status.

A useful record is:

`risk → affected component → impact → mitigation → verification → status`

Unresolved findings should not be silently represented as resolved.

## Avoid unsupported claims

Terms such as:

- secure;
- audited;
- formally verified;
- production-safe;
- trustless;
- private;
- anonymous;

should be used only when the scope and supporting evidence are clearly documented.

Prefer precise statements such as:

- "tested against these vectors";
- "interoperable with this implementation";
- "no known issue was found in these tests";
- "read-only with respect to this interface";
- "does not intentionally persist this data."

## Independent review

Maintainer review, automated tooling, testing, and AI-assisted review are useful but are not substitutes for independent security review where the risk warrants it.

A formal audit should only be claimed when an identifiable independent audit has actually occurred.

## Remediation

When a security issue is discovered:

1. understand and reproduce the issue;
2. determine affected components and versions;
3. limit unnecessary disclosure while remediation is in progress;
4. implement the smallest appropriate fix;
5. add regression coverage when practical;
6. document remaining risk;
7. coordinate disclosure when appropriate.

## Project-specific documentation

Individual repositories may define more specific security requirements.

Project-specific documentation takes precedence over these general principles where the two differ.

## Broader engineering principles

Security exists within a broader set of engineering values.

Projects maintained by 0xterricola generally aim to advance censorship resistance, free and open-source software, privacy, security, self-custody, and user sovereignty where those properties are relevant to the project.

These principles are influenced by the Ethereum Foundation's CROPS framework — Censorship Resistance, Open Source, Privacy, and Security — but are applied independently and do not imply affiliation with or endorsement by the Ethereum Foundation.

These are design goals rather than guarantees. Individual projects may involve tradeoffs, incomplete implementations, external dependencies, or experimental functionality that limit one or more of these properties.
