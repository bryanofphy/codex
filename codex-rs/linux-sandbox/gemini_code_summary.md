# Codex Linux Sandbox

## Overview
`codex-linux-sandbox` implements sandboxing features specifically for Linux systems. It leverages Linux kernel features like Landlock to restrict the access rights of processes.

## Responsibility
- **Filesystem Isolation:** Uses Landlock (`landlock.rs`) to restrict file system access.
- **Mount Management:** Handles mount points (`mounts.rs`) for the sandbox environment.
- **Process Entry:** `linux_run_main.rs` likely serves as the entry point for running a process inside the sandbox.

## Key Files
- **`src/landlock.rs`**: Interface to the Linux Landlock LSM.
- **`src/linux_run_main.rs`**: Main logic for setting up and running a sandboxed process.
