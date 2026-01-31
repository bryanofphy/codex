# Codex Exec

## Overview
`codex-exec` provides functionality for executing commands and processing the resulting events. It seems to be capable of running as a standalone CLI tool or used as a library to drive command execution with structured output handling.

## Responsibility
- **Command Execution:** Runs processes/commands.
- **Event Processing:** Processes execution events, supporting both human-readable (`event_processor_with_human_output.rs`) and JSONL (`event_processor_with_jsonl_output.rs`) formats.
- **CLI Interface:** `cli.rs` and `main.rs` suggest a command-line interface for invoking execution tasks directly.

## Key Files
- **`src/lib.rs`**: Core library entry point.
- **`src/exec_events.rs`**: Definitions of events generated during execution.
- **`src/event_processor.rs`**: Trait or base logic for processing execution events.
