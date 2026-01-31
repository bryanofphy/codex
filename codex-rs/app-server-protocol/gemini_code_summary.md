# Codex App Server Protocol

## Overview
`codex-app-server-protocol` defines the communication protocol used by the Codex App Server. It appears to utilize JSON-RPC.

## Responsibility
- **Protocol Definition:** Defines the messages and structures used for communication (`protocol/`).
- **JSON-RPC:** Implements or wrappers JSON-RPC functionality (`jsonrpc_lite.rs`).

## Key Files
- **`src/lib.rs`**: Library entry point.
- **`src/protocol/`**: Directory containing protocol definitions.
