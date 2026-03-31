# konkud

## How to Install GitHub Copilot on the Terminal

GitHub Copilot CLI brings AI-powered assistance directly to your terminal. Follow the steps below for your operating system.

---

### Prerequisites

- An active [GitHub Copilot subscription](https://github.com/features/copilot) (Individual, Pro, Business, or Enterprise)
- Node.js v22 or higher and npm v10 or higher (for the npm installation method)
- (Windows only) PowerShell v6 or higher, or use WSL for the best experience

---

### Installation

#### Linux

```bash
# Option 1: Official install script (Ubuntu/Debian and other distros)
curl -fsSL https://gh.io/copilot-install | bash

# Option 2: npm (requires Node.js ≥ 22)
npm install -g @github/copilot-cli
```

#### macOS

```bash
# Option 1: Homebrew
brew install gh
gh extension install github/gh-copilot

# Option 2: Official install script
curl -fsSL https://gh.io/copilot-install | bash

# Option 3: npm (requires Node.js ≥ 22)
npm install -g @github/copilot-cli
```

#### Windows

```powershell
# Option 1: WinGet (recommended for native Windows)
winget install GitHub.Copilot

# Option 2: npm (requires Node.js ≥ 22)
npm install -g @github/copilot-cli
```

> **WSL users (Windows):** Run the same install script as Linux inside your WSL terminal.

---

### Authentication

After installation, authenticate with your GitHub account:

```bash
# Log in via GitHub CLI (if using the gh extension)
gh auth login

# Or launch Copilot and use the /login command
copilot
# Then type: /login
```

Follow the browser prompts to complete the OAuth flow.

---

### Basic Usage

```bash
# Start an interactive Copilot session
copilot

# Pass a one-off prompt directly
copilot -p "explain this codebase"

# List all available commands
copilot /help
```

---

### More Resources

- [GitHub Docs – Set up Copilot CLI](https://docs.github.com/en/copilot/how-tos/copilot-cli/set-up-copilot-cli)
- [GitHub Blog – Copilot CLI: How to get started](https://github.blog/ai-and-ml/github-copilot/github-copilot-cli-how-to-get-started/)
- [Codecademy – How to Install and Use GitHub Copilot CLI](https://www.codecademy.com/article/how-to-install-and-use-github-copilot-cli)