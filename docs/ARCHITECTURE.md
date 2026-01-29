# Architecture Overview

Project Paperclip is a local-first AI assistant that prioritizes privacy, transparency, and
user control. This document captures the high-level architecture to guide early development.

## Core components
1. **Desktop Client**
   - UI for conversation, tasks, and settings.
   - Secure permissions panel for tool access.
2. **Local AI Runtime**
   - Manages model loading, inference, and embeddings.
   - Runs locally; optional remote model endpoints are opt-in.
3. **Tool Runner**
   - Executes OS and app integrations with a permissioned API.
   - Provides audit logs for actions performed.
4. **Knowledge Store**
   - Local vector index and metadata store.
   - Ingestion pipeline for files (PDF, Markdown, etc.).

## Data flow
1. User input enters the desktop client.
2. Requests are routed to the local AI runtime.
3. The assistant may call tools via the Tool Runner (with explicit permissions).
4. Results are displayed and optionally stored locally.

## Security principles
- Default to least privilege for tool access.
- Provide transparent logs of actions.
- Avoid background network calls unless explicitly configured.
