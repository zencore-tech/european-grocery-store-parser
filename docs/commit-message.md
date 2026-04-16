
Welcome to the project! To maintain a clean and readable commit history, we follow these guidelines.

---

## 📝 Commit Message Format

We use the **Conventional Commits** specification. Every commit message is automatically validated via `husky`.

**Pattern:**
`<type>: <description>`

### Allowed Types:

| Type | Description |
| :--- | :--- |
| ✨ **feat** | A new feature |
| 🐛 **fix** | A bug fix |
| ⚡ **perf** | A code change that improves performance |
| 📚 **docs** | Documentation only changes |
| 🎨 **style** | Changes that do not affect the meaning of the code (white-space, formatting, etc) |
| ♻️ **refactor** | A code change that neither fixes a bug nor adds a feature |
| ✅ **test** | Adding missing tests or correcting existing tests |
| 🏗 **build** | Changes that affect the build system or external dependencies (pnpm, docker) |
| 🧹 **chore** | Other changes that don't modify src or test files (husky config, gitignore) |
| 🚀 **ci** | Changes to our CI configuration files and scripts (GitHub Actions, deploy scripts) |

---

## 💡 Examples

### ✅ Good:
- `feat: implement Lidl price parser logic`
- `fix: handle connection timeout on worker startup`
- `docs: update commit message guidelines`
- `chore: initial husky hooks setup`

### ❌ Bad:
- `added some code` (no type)
- `fix: fixed bug` (too vague)
- `FEAT: NEW PARSER` (must be lowercase)

---

## 🚀 Workflow (GitFlow)

1. **Main branch** — stable production-ready code only.
2. **Develop branch** — main integration branch for development.
3. **Feature branches** — create a new branch from `develop` for every task:
    - `feat/parser-lidl`
    - `fix/auth-header`
    - `docs/api-description`

---

## 🛠 Automation
The project uses **Husky**. If your commit message doesn't match the format, the commit will be rejected. This ensures our `git log` stays professional and easy to navigate.