# Codex TypeScript SDK

## Overview
This directory contains the official TypeScript SDK for Codex. It allows developers to integrate Codex's capabilities—such as executing commands, managing conversation threads, and handling events—directly into TypeScript or JavaScript applications.

## Responsibility
- **Client Interface:** Provides a typed interface (`Codex` class) for interacting with the Codex backend.
- **Thread Management:** Manages conversational contexts and turns via `Thread` and `TurnOptions`.
- **Execution Control:** Handles command execution and output streaming through `Exec` and related modules.
- **Event Handling:** exposes an event-driven architecture for monitoring system state and task progress.

## Key Files
- **`src/index.ts`**: The main entry point, exporting the public API.
- **`src/codex.ts`**: Defines the main `Codex` client class.
- **`src/thread.ts`**: Implements conversation threads, managing state and history.
- **`src/exec.ts`**: Handles the execution of commands and processes.
- **`src/events.ts`**: Defines the event system for the SDK.
- **`src/items.ts`**: Likely defines data structures for items returned or processed by the SDK.

## Usage
Developers import the `Codex` class to initialize a client, create threads, and send natural language instructions or commands to be executed by the Codex engine.
