# Codex CLI Wrapper

## Overview
This directory contains the Node.js-based CLI wrapper for Codex. Its primary purpose is to serve as a unified entry point that abstracts away the platform-specific execution of the underlying native Rust binaries.

## Responsibility
- **Platform Detection:** Detects the user's operating system (Linux, macOS, Windows) and architecture (x64, arm64).
- **Binary Resolution:** Locates the correct pre-compiled native binary (e.g., `codex` or `codex.exe`) within the `vendor/` directory based on the detected platform.
- **Process Management:** Spawns the native binary as a child process, forwards environment variables, manages `PATH`, and handles signal propagation (SIGINT, SIGTERM) to ensure graceful shutdowns.
- **Package Management:** Includes scripts for building the NPM package, managing native dependencies, and containerized builds.

## Key Files
- **`bin/codex.js`**: The main entry point. It handles the logic for platform detection, binary path resolution, and spawning the native process.
- **`scripts/`**: Contains utility scripts for the build process:
  - `build_npm_package.py`: Automates the creation of the NPM package.
  - `install_native_deps.py`: Handles fetching or installing native dependencies.
  - `build_container.sh` / `run_in_container.sh`: Helpers for containerized development and builds.

## Usage
This package is typically installed via a package manager like `npm` or `bun`. When the user runs `codex`, this Node.js wrapper executes, seamlessly launching the appropriate high-performance Rust binary for their system.
