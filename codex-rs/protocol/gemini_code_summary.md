# Codex Protocol

## Overview
The `codex-protocol` crate defines the shared data structures, message types, and contracts used for communication between different parts of the Codex system (e.g., between the CLI/TUI and the App Server, or internally between components).

## Responsibility
- **Data Models:** Defines core domain objects like `ThreadId` (`thread_id.rs`), `MessageHistory` (`message_history.rs`), and `Items` (`items.rs`).
- **Communication Contract:** Defines the messages exchanged within the system (`protocol.rs`).
- **Configuration Types:** Shared types for configuration (`config_types.rs`).
- **Approval Types:** Definitions for approval requests and responses (`approvals.rs`).

## Key Files
- **`src/protocol.rs`**: The central definition of the protocol messages.
- **`src/models.rs`**: General shared data models.
- **`src/items.rs`**: Definitions for items (likely units of work or data in the UI).
- **`src/approvals.rs`**: Types for handling user approvals.

## Usage
This crate is a dependency for almost all other major crates in the workspace (`core`, `app-server`, `tui`, `cli`), ensuring type consistency across the system.
