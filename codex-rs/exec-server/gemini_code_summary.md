# Codex Exec Server

## Overview
`codex-exec-server` acts as a server component for command execution. It abstracts the platform-specific details of running commands, potentially in isolated environments.

## Responsibility
- **Execution Service:** Provides a service interface for executing commands.
- **Platform Abstraction:** The `posix` module suggests support for POSIX-compliant systems.

## Key Files
- **`src/lib.rs`**: Library logic.
- **`src/posix.rs`**: POSIX-specific execution logic.
