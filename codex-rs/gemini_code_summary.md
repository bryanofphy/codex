# Codex Rust Core (`codex-rs`)

## Overview
`codex-rs` is the root of the Rust workspace that powers the core logic of Codex. It is a monorepo containing multiple crates that handle everything from the command-line interface and terminal UI to the backend application server, protocol definitions, and platform-specific sandboxing.

## Structure
The workspace is organized into numerous crates (packages), each with a specific responsibility.

## Key Member Crates

### Core Application & Interface
- **`cli`**: The Rust entry point for the Codex command-line application.
- **`tui`**: Implements the rich Terminal User Interface.
- **`app-server`**: The central backend server that coordinates logic, state, and client interactions.
- **`codex-api`**: Defines the high-level API for interacting with Codex.

### Logic & Protocol
- **`core`**: Contains the primary business logic and domain models.
- **`protocol`**: Defines the communication protocols used between different components (e.g., between the CLI and the App Server).
- **`mcp-server`**: Implements the Model Context Protocol (MCP) server functionality.
- **`mcp-types`**: Shared types for MCP.

### Infrastructure & execution
- **`exec` / `exec-server`**: Handles the actual execution of commands and tasks.
- **`execpolicy`**: Enforces security policies regarding what commands can be run.
- **`linux-sandbox` / `windows-sandbox-rs`**: Platform-specific sandboxing implementations to ensure safe execution.
- **`network-proxy`**: Manages network interactions and proxying.

### Clients & Integrations
- **`codex-client`**: Internal client library for the backend.
- **`ollama` / `chatgpt` / `lmstudio`**: Integrations with various LLM providers.
- **`cloud-tasks`**: Integrations for cloud-based task offloading.

## Build
This project uses `cargo` for building and testing. It defines a workspace in `Cargo.toml` that aggregates all member crates.
