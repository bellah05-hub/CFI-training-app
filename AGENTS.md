# AGENTS.md

## Cursor Cloud specific instructions

### Repository State

This is a **greenfield project** — the repository currently contains only a `README.md` describing the product vision (a CFI check-ride training app). There is no source code, no dependencies, no build system, and no runnable application yet.

### Available Environment

- **Node.js**: v22 (via nvm)
- **Python**: 3.12
- **Package managers**: npm, pnpm, yarn are available
- **OS**: Ubuntu (Linux)

### Development Notes

- No lint, test, or build commands exist yet. Future agents should check for `package.json`, `requirements.txt`, `pyproject.toml`, or similar dependency files before attempting to install or run anything.
- The update script is a no-op (`echo`) since there are no dependencies to install. Once code is added, the update script should be changed to the appropriate dependency install command (e.g., `npm install`, `pip install -r requirements.txt`).
