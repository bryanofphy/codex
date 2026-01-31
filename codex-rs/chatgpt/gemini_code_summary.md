# Codex ChatGPT Integration

## Overview
`codex-chatgpt` implements the integration with OpenAI's ChatGPT. It allows Codex to use ChatGPT as a model provider.

## Responsibility
- **Model Integration:** Connects to ChatGPT APIs (`chatgpt_client.rs`, `connectors.rs`).
- **Command Application:** `apply_command.rs` likely handles formatting commands for the model.
- **Token Management:** Handles token counting or management (`chatgpt_token.rs`).

## Key Files
- **`src/chatgpt_client.rs`**: The core client for ChatGPT.
