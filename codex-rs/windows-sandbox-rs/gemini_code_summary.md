# Codex Windows Sandbox

## Overview
`codex-windows-sandbox-rs` implements comprehensive sandboxing and security isolation for Windows. It manages user identities, access control lists (ACLs), firewall rules, and process tokens to secure execution.

## Responsibility
- **User Management:** Manages sandbox user accounts (`sandbox_users.rs`, `hide_users.rs`).
- **Access Control:** Manipulates Windows ACLs (`acl.rs`, `read_acl_mutex.rs`) to restrict access.
- **Network Security:** Configures firewall rules (`firewall.rs`).
- **Process Isolation:** Manages process tokens and identities (`token.rs`, `identity.rs`).
- **Setup:** Orchestrates the setup of the sandbox environment (`setup_orchestrator.rs`).

## Key Files
- **`src/setup_main_win.rs`**: Entry point for sandbox setup.
- **`src/winutil.rs`**: Windows API utilities.
- **`src/firewall.rs`**: Firewall configuration logic.
