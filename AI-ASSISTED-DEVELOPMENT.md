# AI-Assisted Development

Projects maintained by **0xterricola** may use artificial intelligence tools extensively throughout development.

This disclosure is intended to make that development process explicit.

## Uses

AI assistance may be used for:

- code generation;
- code modification;
- debugging;
- refactoring;
- test generation;
- documentation;
- standards and API research;
- implementation planning;
- threat modeling;
- security review support;
- static reasoning;
- build and tooling assistance;
- analysis of logs and compiler output;
- rapid prototyping and proof-of-concept development;
- exploring implementation approaches and technical ideas;
- iterative experimentation and refinement.

The amount of AI assistance may vary substantially between repositories and commits.

## Development workflow

AI tools are also used to shorten the path from an idea to something that can be tested.

This may include rapidly producing prototypes, proof-of-concept implementations, experiments, integration tests, or exploratory tooling in order to investigate whether an idea is technically viable.

Development may proceed iteratively:

`idea → prototype → test → investigate → revise → repeat`

Early implementations may therefore prioritize learning, experimentation, and validation before architecture, interfaces, documentation, or security properties are finalized.

Experimental or proof-of-concept code should not be interpreted as production-ready solely because it is functional.

As an idea matures, implementation assumptions, failure modes, dependencies, test coverage, and security implications should be examined more closely and documented where appropriate.

AI assistance is used to accelerate this investigative process, not to replace technical understanding or validation.

## Responsibility

AI-generated or AI-assisted output is treated as untrusted development input.

AI systems can produce:

- incorrect code;
- nonexistent APIs;
- incomplete reasoning;
- insecure assumptions;
- subtle cryptographic mistakes;
- incorrect protocol interpretations;
- insufficient tests;
- misleading documentation.

AI assistance does not transfer responsibility for committed code to the AI system.

The maintainer decides what is accepted into the repository and remains responsible for reviewing, testing, modifying, rejecting, or reverting generated output.

## Security

AI assistance is not:

- a security audit;
- independent security review;
- formal verification;
- proof of cryptographic correctness;
- evidence that a project is vulnerability-free.

Security-sensitive AI-assisted changes should receive the same or greater scrutiny as manually authored changes.

For cryptographic and wallet-related code, preference should be given to standards, reference implementations, test vectors, interoperability testing, regression testing, and human review.

## Human and independent review

Human review remains important, especially for:

- cryptography;
- signing;
- key management;
- wallet behavior;
- authentication;
- serialization;
- protocol parsing;
- network interfaces;
- access control;
- security boundaries.

Where appropriate, independent review should be sought separately from AI-assisted development.

## Secrets and sensitive information

Private keys, seed phrases, passwords, authentication tokens, API credentials, and equivalent secrets should not intentionally be supplied to AI systems as part of project development.

Logs and debugging output should be reviewed for sensitive information before being shared externally.

## Attribution

Individual AI-assisted lines or commits may not be separately labeled.

This document provides a repository-wide disclosure that AI may have materially assisted the development process.

Repositories may provide more detailed disclosures when useful.

## Transparency

The goal of this disclosure is not to imply that AI-assisted software is inherently secure or insecure.

It is to describe the development process accurately so that contributors, reviewers, and users can evaluate the software with appropriate context.
