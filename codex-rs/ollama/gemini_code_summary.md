# Codex Ollama Integration

## Overview
`codex-ollama` provides integration with Ollama, enabling Codex to utilize local LLMs hosted by Ollama.

## Responsibility
- **Local Inference:** Connects to a local Ollama instance (`client.rs`).
- **Model Pulling:** functionality to pull models (`pull.rs`).
- **Parsing:** Parses Ollama responses (`parser.rs`).

## Key Files
- **`src/client.rs`**: The Ollama client implementation.
