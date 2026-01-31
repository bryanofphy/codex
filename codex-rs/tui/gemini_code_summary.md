# Codex TUI (Terminal User Interface)

## Overview
This crate implements the rich Terminal User Interface for Codex. It provides the visual, interactive environment where users chat with the AI, review code changes, and manage execution.

## Responsibility
- **UI Rendering:** Renders the application state to the terminal using components like chat widgets (`chatwidget/`), execution cells (`exec_cell/`), and status bars.
- **Event Handling:** Manages user input (keyboard events) and application events (`app_event.rs`, `app.rs`).
- **Markdown Rendering:** specialized logic for rendering Markdown and code blocks in the terminal (`markdown_render.rs`, `markdown.rs`).
- **Feature Integration:** UI front-ends for file search, git diffs, and slash commands.
- **State Management:** `app.rs` likely holds the TUI-specific application state.

## Key Files & Modules
- **`src/app.rs`**: The main TUI application logic and event loop.
- **`src/tui.rs`**: Core TUI setup and teardown.
- **`src/chatwidget/`**: Components for the chat interface.
- **`src/exec_cell/`**: Components for displaying executed commands and outputs.
- **`src/render/`**: Rendering utilities.
- **`src/markdown_render.rs`**: Handles the visual presentation of Markdown text.

## Usage
This crate is typically invoked by the `cli` crate when the user starts Codex in interactive mode.
