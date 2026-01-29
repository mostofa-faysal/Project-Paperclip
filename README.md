# Project-Paperclip
An open-source, local-first AI assistant for your PC.

## Vision
Project Paperclip aims to provide a privacy-respecting AI companion that runs fully on your
computer. It should help with everyday workflows (notes, reminders, system automation, and
knowledge retrieval) without sending your data to external servers.

## Goals
- **Local-first**: run models and services on-device whenever possible.
- **Extensible**: plugin architecture for tools, integrations, and skills.
- **Transparent**: open source, auditable components and clear data handling.
- **Cross-platform**: target Windows, macOS, and Linux.

## Roadmap (draft)
1. **MVP**
   - Local model runtime (LLM + speech optional).
   - Desktop UI shell.
   - Tool runner with a safe, permissioned API.
2. **Automation**
   - OS-level actions (files, clipboard, app launching).
   - Scheduled tasks and reminders.
3. **Knowledge**
   - Local vector index + document ingestion.
   - Search and summarization over personal files.
4. **Ecosystem**
   - Plugin SDK + marketplace pattern.
   - Community-contributed integrations.

## Repository layout (proposed)
- `apps/` – desktop client(s).
- `services/` – local AI/runtime services.
- `packages/` – shared libraries (SDK, UI components, core logic).
- `docs/` – architecture, contributing, and specs.

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines, and read the
[Architecture Overview](docs/ARCHITECTURE.md) for design principles.

## License
MIT. See [LICENSE](LICENSE).
