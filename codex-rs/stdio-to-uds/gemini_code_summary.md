# Codex Stdio to UDS

## Overview
`codex-stdio-to-uds` is a utility that bridges Standard Input/Output (stdio) to a Unix Domain Socket (UDS). This is often used for inter-process communication where one process expects a socket and another speaks stdio.

## Responsibility
- **Stream Bridging:** Forwards data between stdio and a socket.

## Key Files
- **`src/main.rs`**: Binary entry point.
