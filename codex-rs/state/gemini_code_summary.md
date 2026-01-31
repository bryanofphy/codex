# Codex State

## Overview
`codex-state` manages persistent application state, likely using a local database (SQLite/DuckDB etc.).

## Responsibility
- **Persistence:** Manages a log database (`log_db.rs`).
- **Migrations:** Handles schema migrations (`migrations.rs`).
- **Paths:** Manages state file paths (`paths.rs`).

## Key Files
- **`src/lib.rs`**: Library entry point.
- **`src/log_db.rs`**: Database interaction logic.
