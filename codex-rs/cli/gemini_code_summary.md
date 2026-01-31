# Codex CLI (Rust)

## Overview
This crate implements the native Rust command-line interface for Codex. It is the binary that is eventually spawned by the Node.js wrapper (in `codex-cli`). It handles the user's direct interaction in the terminal, including login, command execution, and launching the TUI.

## Responsibility
- **Entry Point:** `main.rs` parses command-line arguments and flags.
- **Authentication:** `login.rs` manages user authentication flows.
- **Debug & Diagnostics:** Includes tools for debugging the sandbox (`debug_sandbox.rs`) and checking the environment.
- **MCP Integration:** `mcp_cmd.rs` provides commands related to the Model Context Protocol.
- **Platform Utils:** Handles specific path conversions for WSL (`wsl_paths.rs`).

## Key Files
- **`src/main.rs`**: Main application entry point.
- **`src/login.rs`**: Authentication logic.
- **`src/mcp_cmd.rs`**: Subcommands for MCP operations.
- **`src/debug_sandbox.rs`**: Sandbox debugging utilities.

## Usage
This binary is usually renamed to `codex` (or `codex.exe`) and placed in a vendor directory where the Node.js wrapper finds it.
