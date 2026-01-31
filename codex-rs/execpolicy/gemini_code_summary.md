# Codex Exec Policy

## Overview
`codex-execpolicy` implements the policy engine that governs which commands are allowed to be executed by the system. It parses policy rules and makes decisions on whether to allow or deny specific executions.

## Responsibility
- **Policy Enforcement:** Checks execution requests against defined rules (`execpolicycheck.rs`, `decision.rs`).
- **Rule Parsing:** Parses policy definitions (`parser.rs`, `rule.rs`, `policy.rs`).
- **Error Handling:** Defines errors related to policy violations (`error.rs`).

## Key Files
- **`src/execpolicycheck.rs`**: Core logic for checking a command against the policy.
- **`src/policy.rs`**: Definition of the policy structure.
