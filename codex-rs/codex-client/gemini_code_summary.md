# Codex Client

## Overview
`codex-client` is a general-purpose client library for interacting with Codex services. It handles the low-level details of making requests, handling Server-Sent Events (SSE), and managing retries.

## Responsibility
- **HTTP Transport:** Manages HTTP connections (`transport.rs`).
- **SSE Support:** Handles Server-Sent Events for streaming responses (`sse.rs`).
- **Resilience:** Implements retry logic (`retry.rs`) for robust communication.
- **Telemetry:** Captures telemetry data (`telemetry.rs`).

## Key Files
- **`src/lib.rs`**: Library entry point.
- **`src/default_client.rs`**: A default client implementation.
