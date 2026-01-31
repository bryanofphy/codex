# Codex App Server

## Overview
The `app-server` crate is the backend service for Codex. It acts as the central coordinator that processes messages, manages application state, and handles API requests. It can operate as a standalone server.

## Responsibility
- **Message Processing:** Receives and processes incoming messages via `message_processor.rs` and `codex_message_processor.rs`.
- **API Handling:** Exposes APIs for configuration (`config_api.rs`) and other services.
- **Tool Management:** Manages dynamic tools (`dynamic_tools.rs`) available to the system.
- **Search:** Implements fuzzy file search capabilities (`fuzzy_file_search.rs`).

## Key Files
- **`src/main.rs`**: The entry point for the server executable.
- **`src/lib.rs`**: The library definition, exposing the server's functionality.
- **`src/codex_message_processor.rs`**: Specific logic for processing Codex-related messages.
- **`src/message_processor.rs`**: General message processing infrastructure.
- **`src/outgoing_message.rs`**: Defines the structure and handling of messages sent back to clients.

## Dependencies
It relies heavily on `codex-core` for business logic and `codex-protocol` for data structures.
