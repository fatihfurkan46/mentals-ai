# Architecture

- `src/` - the runtime: mental loop, tool dispatch and prompt assembly.
- `agents/` - example agent definitions.
- `native_tools.toml` - the tools exposed to the model.
- `mentals_system.prompt` - the system prompt the runtime sends before every turn.

The runtime is a single native binary; the prompt and tool table are data files so a new agent is a
directory, not a rebuild.
