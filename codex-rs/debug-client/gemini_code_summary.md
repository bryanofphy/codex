# Codex Debug Client

## Overview
`codex-debug-client` is a standalone CLI tool or client module used for debugging the Codex system. It likely connects to a running Codex instance to inspect state or drive execution.

## Responsibility
- **Debugging Interface:** Provides commands (`commands.rs`) to interact with the system for debugging.
- **State Inspection:** `state.rs` suggests capabilities to view or manipulate internal state.
- **Input/Output:** Handles reading input and formatting output (`reader.rs`, `output.rs`).

## Key Files
- **`src/main.rs`**: CLI entry point.
- **`src/client.rs`**: Client logic for connecting to the debug target.
