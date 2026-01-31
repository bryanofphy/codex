# Codex Common

## Overview
`codex-common` is a utility crate that contains shared helper functions, types, and logic that are used across multiple crates in the workspace but do not belong to the core business logic or protocol definitions.

## Responsibility
- **Configuration Helpers:** Utilities for handling configuration overrides and summaries (`config_override.rs`, `config_summary.rs`).
- **CLI Helpers:** Shared logic for parsing specific CLI arguments like sandbox modes (`sandbox_mode_cli_arg.rs`) and approval modes (`approval_mode_cli_arg.rs`).
- **Algorithms:** Common algorithms like fuzzy matching (`fuzzy_match.rs`).
- **Formatting:** Utilities for displaying environment variables or time (`format_env_display.rs`, `elapsed.rs`).

## Key Files
- **`src/lib.rs`**: Exports the common utilities.
- **`src/fuzzy_match.rs`**: Implementation of fuzzy matching logic.
- **`src/sandbox_mode_cli_arg.rs`**: Defines how sandbox modes are parsed from the command line.

## Usage
Used as a utility library throughout the `codex-rs` workspace to avoid code duplication for common tasks.
