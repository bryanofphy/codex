# Codex MCP Server

## Overview
`codex-mcp-server` implements the server side of the Model Context Protocol (MCP). It allows Codex to function as an MCP server, exposing its capabilities (tools) to other MCP-compliant clients or agents.

## Responsibility
- **Protocol Implementation:** Handles the MCP message lifecycle (`message_processor.rs`, `outgoing_message.rs`).
- **Tool Exposure:** Hosts and runs tools defined in `tool_handlers/`.
- **Approval Workflows:** Implements human-in-the-loop approval mechanisms for sensitive actions like execution (`exec_approval.rs`) or applying patches (`patch_approval.rs`).
- **Tool Running:** The `codex_tool_runner.rs` is responsible for executing the requested tools.

## Key Files
- **`src/lib.rs`**: Library entry point.
- **`src/message_processor.rs`**: Handles incoming MCP requests.
- **`src/tool_handlers/`**: Directory containing implementations of specific tools.
- **`src/exec_approval.rs`**: Logic for approving execution requests.
