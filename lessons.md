# lessons.md

Environment-specific lessons and constraints. Treat each as a hard constraint.

---

**LESSON-1: Claude Pro subscription and Anthropic API credits are separate**
- Claude Pro ($20/mo) provides access to claude.ai only
- The SDK requires separate API credits from console.anthropic.com
- Never suggest Pro subscription covers SDK usage

---

**LESSON-3: Node.js on this machine — use fnm with Node 20**
- System node is v6.9.5 (too old)
- NVM has only v8.1.4
- Homebrew too old (3.2.13), doesn't support macOS 26
- **Solution:** Always activate fnm before npm/npx:
  ```bash
  export FNM_DIR="$HOME/.local/share/fnm" && eval "$(fnm env)" && fnm use 20
  ```
- Node 20.20.1 is installed via fnm at `/usr/local/bin/fnm`

---

**LESSON-4: Docker is not available on this machine**
- Docker binary at `/usr/local/Cellar/docker/17.06.0/bin/docker` crashes with exit code 139
- Docker Desktop not installed
- Use local alternatives (SQLite, static files) for any dev dependencies
