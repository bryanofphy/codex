# Codex Exec Policy (Legacy)

## Overview
`codex-execpolicy-legacy` contains the previous generation of the execution policy engine. It is likely kept for backward compatibility or reference during migration to the new `execpolicy` crate.

## Responsibility
- **Legacy Policy Checking:** Validates execution calls against a legacy policy format.
- **Argument Resolution:** Resolves and checks command arguments (`arg_resolver.rs`, `arg_matcher.rs`).
- **Policy Parsing:** Parses the old policy format (`policy_parser.rs`).

## Key Files
- **`src/default.policy`**: The default policy file used by this legacy system.
- **`src/execv_checker.rs`**: Logic for checking `execv` calls.
