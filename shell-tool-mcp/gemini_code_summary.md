# Shell Tool MCP Server

## Overview
This directory implements a Model Context Protocol (MCP) server specifically designed for shell integration. It provides tools and capabilities that allow AI agents to interact with the underlying operating system's shell environment safely and effectively.

## Responsibility
- **Shell Interface:** Provides a bridge between MCP clients and the system shell (Bash, etc.).
- **Platform Abstraction:** Handles differences between operating systems (Linux, macOS, Windows) to ensure consistent behavior.
- **Command Execution:** Facilitates the execution of shell commands and capture of their output.

## Key Files
- **`src/index.ts`**: The entry point for the MCP server.
- **`src/bashSelection.ts`**: Implements logic specific to handling Bash shell interactions or selections.
- **`src/platform.ts`**: specific utilities for platform detection and capability checking.
- **`src/osRelease.ts`**: Utilities for parsing OS release information (e.g., `/etc/os-release`).
- **`src/types.ts`**: TypeScript definitions for the internal data structures and MCP interfaces.

## Dependencies
- **Model Context Protocol (MCP):** Relies on the MCP standard to communicate with clients.
- **Node.js Runtime:** Built to run on Node.js.
