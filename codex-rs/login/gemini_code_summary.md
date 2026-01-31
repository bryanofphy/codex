# Codex Login

## Overview
`codex-login` implements advanced authentication flows for the system.

## Responsibility
- **Device Code Auth:** Implements the device code flow (`device_code_auth.rs`).
- **PKCE:** Implements Proof Key for Code Exchange (`pkce.rs`).
- **Local Server:** Runs a local server to capture auth callbacks (`server.rs`).

## Key Files
- **`src/lib.rs`**: Library entry point.
