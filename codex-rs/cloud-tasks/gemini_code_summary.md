# Codex Cloud Tasks

## Overview
`codex-cloud-tasks` implements logic for managing and potentially viewing cloud-based tasks. It includes a UI component, suggesting it might have a TUI or CLI for task inspection.

## Responsibility
- **Task Management:** Handles new tasks (`new_task.rs`).
- **Environment Detection:** Detects environment details (`env_detect.rs`).
- **UI:** Provides a user interface (`ui.rs`, `scrollable_diff.rs`) for interacting with tasks.

## Key Files
- **`src/lib.rs`**: Core logic.
- **`src/app.rs`**: Application state/logic for the task tool.
