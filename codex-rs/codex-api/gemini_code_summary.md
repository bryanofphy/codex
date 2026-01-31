# Codex API

## Overview
`codex-api` provides the high-level API definitions and client logic for interacting with Codex services. It encapsulates authentication, rate limiting, and request handling.

## Responsibility
- **API Endpoints:** Defines API endpoints (`endpoint/`).
- **Request/Response:** Defines request structures (`requests/`) and SSE handling (`sse/`).
- **Authentication:** Manages authentication details (`auth.rs`).
- **Rate Limiting:** Handles rate limit logic (`rate_limits.rs`).

## Key Files
- **`src/lib.rs`**: Library entry point.
- **`src/requests/`**: Directory of request types.
