# Codex Network Proxy

## Overview
`codex-network-proxy` implements a network proxy server, supporting HTTP and SOCKS5, with integrated policy enforcement.

## Responsibility
- **Proxying:** HTTP (`http_proxy.rs`) and SOCKS5 (`socks5.rs`) support.
- **Policy:** Enforces network policies (`network_policy.rs`, `policy.rs`).
- **Admin:** Admin interface (`admin.rs`).

## Key Files
- **`src/main.rs`**: Server entry point.
- **`src/proxy.rs`**: Core proxy logic.
