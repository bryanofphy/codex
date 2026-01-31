# Codex RMCP Client

## Overview
`codex-rmcp-client` is a client library for the Remote Model Context Protocol (RMCP). It handles connection, authentication (OAuth), and communication with remote MCP servers.

## Responsibility
- **Protocol Client:** Implements the client side of RMCP (`rmcp_client.rs`).
- **Authentication:** Handles OAuth login flows (`perform_oauth_login.rs`, `oauth.rs`) and auth status (`auth_status.rs`).
- **Program Resolution:** Resolves programs or tools (`program_resolver.rs`).

## Key Files
- **`src/rmcp_client.rs`**: Core client logic.
- **`src/perform_oauth_login.rs`**: OAuth login flow implementation.
