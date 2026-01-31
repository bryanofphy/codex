# Codex Responses API Proxy

## Overview
`codex-responses-api-proxy` implements a proxy server for the Responses API. It likely sits between clients and the upstream API to handle specific tasks like authentication or logging.

## Responsibility
- **Proxying:** Forwards requests to the API.
- **Auth Handling:** Reads and manages API keys (`read_api_key.rs`).

## Key Files
- **`src/main.rs`**: Server entry point.
- **`src/read_api_key.rs`**: Logic for retrieving API keys.
