# Codex Cloud Tasks Client

## Overview
`codex-cloud-tasks-client` is a client for interacting with a cloud task execution service. It allows Codex to offload or manage tasks in the cloud.

## Responsibility
- **API Access:** Provides access to the cloud tasks API (`api.rs`).
- **HTTP Layer:** Handles HTTP communication (`http.rs`).
- **Testing:** Includes a mock implementation (`mock.rs`) for testing.

## Key Files
- **`src/api.rs`**: API definitions.
