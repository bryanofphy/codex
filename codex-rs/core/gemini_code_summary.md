# Codex Core

## Overview
`codex-core` is the central library containing the primary business logic, domain models, and orchestrators for the Codex system. It serves as the foundation upon which the CLI, App Server, and other components build.

## Responsibility
- **Agent Logic:** Defines the behavior of AI agents (`agent/`).
- **Context Management:** Manages the LLM's context window and session state (`context_manager/`, `codex_thread.rs`, `message_history.rs`).
- **Execution & Safety:** Handles safe execution of shell commands (`exec.rs`, `shell.rs`, `bash.rs`, `powershell.rs`) and enforces security policies (`command_safety/`, `exec_policy.rs`, `sandboxing/`).
- **Tools & MCP:** Manages internal tools (`tools/`) and connections to MCP servers (`mcp/`, `mcp_connection_manager.rs`).
- **Configuration:** Loads and manages application config (`config/`, `config_loader/`).
- **Authentication:** Core auth logic (`auth/`, `auth.rs`).

## Key Files & Modules
- **`src/codex.rs`**: Likely the main facade or coordinator for Codex operations.
- **`src/codex_thread.rs`**: Manages a single conversation thread.
- **`src/exec.rs`**: Core execution engine.
- **`src/shell.rs`**: Abstract shell interface.
- **`src/mcp_connection_manager.rs`**: Manages the lifecycle of MCP connections.
- **`src/api_bridge.rs`**: Bridges the core logic with external APIs.

## Architecture
This crate is highly modular, separating concerns into `agent`, `skills`, `tools`, `tasks`, and `sandboxing` directories to maintain maintainability and testability.
