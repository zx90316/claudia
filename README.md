<div align="center">
  <img src="https://github.com/user-attachments/assets/92fd93ed-e71b-4b94-b270-50684323dd00" alt="Claudia Logo" width="120" height="120">

  <a href="https://claudiacode.com"><h1>Claudia</h1></a>
  
  <p>
    <strong>A powerful GUI app and Toolkit for Claude Code</strong>
  </p>
  <p>
    <strong>Create custom agents, manage interactive Claude Code sessions, run secure background agents, and more.</strong>
  </p>
  
  <p>
    <a href="#features"><img src="https://img.shields.io/badge/Features-✨-blue?style=for-the-badge" alt="Features"></a>
    <a href="#installation"><img src="https://img.shields.io/badge/Install-🚀-green?style=for-the-badge" alt="Installation"></a>
    <a href="#usage"><img src="https://img.shields.io/badge/Usage-📖-purple?style=for-the-badge" alt="Usage"></a>
    <a href="#development"><img src="https://img.shields.io/badge/Develop-🛠️-orange?style=for-the-badge" alt="Development"></a>
  </p>
</div>

![457013521-6133a738-d0cb-4d3e-8746-c6768c82672c](https://github.com/user-attachments/assets/a028de9e-d881-44d8-bae5-7326ab3558b9)

https://github.com/user-attachments/assets/bf0bdf9d-ba91-45af-9ac4-7274f57075cf

> [!TIP]
> **⭐ Star the repo and follow [@getAsterisk](https://x.com/getAsterisk) on X for early access to `asteria-swe-v0`**.

## 🌟 Overview

**Claudia** is a powerful desktop application that transforms how you interact with Claude Code. Built with Tauri 2, it provides a beautiful GUI for managing your Claude Code sessions, creating custom agents, tracking usage, and much more.

Think of Claudia as your command center for Claude Code - bridging the gap between the command-line tool and a visual experience that makes AI-assisted development more intuitive and productive.

## 📋 Table of Contents

- [🌟 Overview](#-overview)
- [✨ Features](#-features)
  - [🗂️ Project & Session Management](#️-project--session-management)
  - [🤖 CC Agents](#-cc-agents)
  
  - [📊 Usage Analytics Dashboard](#-usage-analytics-dashboard)
  - [🔌 MCP Server Management](#-mcp-server-management)
  - [⏰ Timeline & Checkpoints](#-timeline--checkpoints)
  - [📝 CLAUDE.md Management](#-claudemd-management)
- [📖 Usage](#-usage)
  - [Getting Started](#getting-started)
  - [Managing Projects](#managing-projects)
  - [Creating Agents](#creating-agents)
  - [Tracking Usage](#tracking-usage)
  - [Working with MCP Servers](#working-with-mcp-servers)
- [🚀 Installation](#-installation)
- [🔨 Build from Source](#-build-from-source)
- [🛠️ Development](#️-development)
- [🔒 Security](#-security)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [🙏 Acknowledgments](#-acknowledgments)

## ✨ Features

### 🗂️ **Project & Session Management**
- **Visual Project Browser**: Navigate through all your Claude Code projects in `~/.claude/projects/`
- **Session History**: View and resume past coding sessions with full context
- **Smart Search**: Find projects and sessions quickly with built-in search
- **Session Insights**: See first messages, timestamps, and session metadata at a glance

### 🤖 **CC Agents**
- **Custom AI Agents**: Create specialized agents with custom system prompts and behaviors
- **Agent Library**: Build a collection of purpose-built agents for different tasks
- **Background Execution**: Run agents in separate processes for non-blocking operations
- **Execution History**: Track all agent runs with detailed logs and performance metrics



### 📊 **Usage Analytics Dashboard**
- **Cost Tracking**: Monitor your Claude API usage and costs in real-time
- **Token Analytics**: Detailed breakdown by model, project, and time period
- **Visual Charts**: Beautiful charts showing usage trends and patterns
- **Export Data**: Export usage data for accounting and analysis

### 🔌 **MCP Server Management**
- **Server Registry**: Manage Model Context Protocol servers from a central UI
- **Easy Configuration**: Add servers via UI or import from existing configs
- **Connection Testing**: Verify server connectivity before use
- **Claude Desktop Import**: Import server configurations from Claude Desktop

### ⏰ **Timeline & Checkpoints**
- **Session Versioning**: Create checkpoints at any point in your coding session
- **Visual Timeline**: Navigate through your session history with a branching timeline
- **Instant Restore**: Jump back to any checkpoint with one click
- **Fork Sessions**: Create new branches from existing checkpoints
- **Diff Viewer**: See exactly what changed between checkpoints

### 📝 **CLAUDE.md Management**
- **Built-in Editor**: Edit CLAUDE.md files directly within the app
- **Live Preview**: See your markdown rendered in real-time
- **Project Scanner**: Find all CLAUDE.md files in your projects
- **Syntax Highlighting**: Full markdown support with syntax highlighting

## 📖 Usage

### Getting Started

1. **Launch Claudia**: Open the application after installation
2. **Welcome Screen**: Choose between CC Agents or CC Projects
3. **First Time Setup**: Claudia will automatically detect your `~/.claude` directory

### Managing Projects

```
CC Projects → Select Project → View Sessions → Resume or Start New
```

- Click on any project to view its sessions
- Each session shows the first message and timestamp
- Resume sessions directly or start new ones

### Creating Agents

```
CC Agents → Create Agent → Configure → Execute
```

1. **Design Your Agent**: Set name, icon, and system prompt
2. **Configure Model**: Choose between available Claude models
3. **Set Permissions**: Configure file read/write and network access
4. **Execute Tasks**: Run your agent on any project

### Tracking Usage

```
Menu → Usage Dashboard → View Analytics
```

- Monitor costs by model, project, and date
- Export data for reports
- Set up usage alerts (coming soon)

### Working with MCP Servers

```
Menu → MCP Manager → Add Server → Configure
```

- Add servers manually or via JSON
- Import from Claude Desktop configuration
- Test connections before using

## 🚀 Installation

### Prerequisites

- **Claude Code CLI**: Install from [Claude's official site](https://claude.ai/code)

### Release Executables Will Be Published Soon

## 🔨 Build from Source

### Prerequisites

Before building Claudia from source, ensure you have the following installed:

#### System Requirements

- **Operating System**: Windows 10/11, macOS 11+, or Linux (Ubuntu 20.04+)
- **RAM**: Minimum 4GB (8GB recommended)
- **Storage**: At least 1GB free space

#### Required Tools

1. **Rust** (1.70.0 or later)
   ```bash
   # Install via rustup
   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
   ```
   **windows**
   https://www.rust-lang.org/zh-TW/learn/get-started

2. **Bun** (latest version)
   ```bash
   # Install bun
   curl -fsSL https://bun.sh/install | bash
   ```
   **windows**
   ''''bash
   powershell -c "irm bun.sh/install.ps1 | iex"
   '''


3. **Git**
   ```bash
   # Usually pre-installed, but if not:
   # Ubuntu/Debian: sudo apt install git
   # macOS: brew install git
   # Windows: Download from https://git-scm.com
   ```

4. **Claude Code CLI**
   - Download and install from [Claude's official site](https://claude.ai/code)
   - Ensure `claude` is available in your PATH
   
   **windows**
   使用下方說明安裝Claude Code
   https://github.com/somersby10ml/win-claude-code

#### Platform-Specific Dependencies

**Linux (Ubuntu/Debian)**
```bash
# Install system dependencies
sudo apt update
sudo apt install -y \
  libwebkit2gtk-4.1-dev \
  libgtk-3-dev \
  libayatana-appindicator3-dev \
  librsvg2-dev \
  patchelf \
  build-essential \
  curl \
  wget \
  file \
  libssl-dev \
  libxdo-dev \
  libsoup-3.0-dev \
  libjavascriptcoregtk-4.1-dev
```

**macOS**
```bash
# Install Xcode Command Line Tools
xcode-select --install

# Install additional dependencies via Homebrew (optional)
brew install pkg-config
```

**Windows**
- Install [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)
- Install [WebView2](https://developer.microsoft.com/microsoft-edge/webview2/) (usually pre-installed on Windows 11)

### Build Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/getAsterisk/claudia.git
   cd claudia
   ```

2. **Install Frontend Dependencies**
   ```bash
   bun install
   ```

3. **Build the Application**
   
   **For Development (with hot reload)**
   ```bash
   bun run tauri dev
   ```
   
   **For Production Build**
   ```bash
   # Build the application
   bun run tauri build
   
   # The built executable will be in:
   # - Linux: src-tauri/target/release/bundle/
   # - macOS: src-tauri/target/release/bundle/
   # - Windows: src-tauri/target/release/bundle/
   ```

4. **Platform-Specific Build Options**
   
   **Debug Build (faster compilation, larger binary)**
   ```bash
   bun run tauri build --debug
   ```
   
   **Build without bundling (creates just the executable)**
   ```bash
   bun run tauri build --no-bundle
   ```
   
   **Universal Binary for macOS (Intel + Apple Silicon)**
   ```bash
   bun run tauri build --target universal-apple-darwin
   ```

### Troubleshooting

#### Common Issues

1. **"cargo not found" error**
   - Ensure Rust is installed and `~/.cargo/bin` is in your PATH
   - Run `source ~/.cargo/env` or restart your terminal

2. **Linux: "webkit2gtk not found" error**
   - Install the webkit2gtk development packages listed above
   - On newer Ubuntu versions, you might need `libwebkit2gtk-4.0-dev`

3. **Windows: "MSVC not found" error**
   - Install Visual Studio Build Tools with C++ support
   - Restart your terminal after installation

4. **"claude command not found" error**
   - Ensure Claude Code CLI is installed and in your PATH
   - Test with `claude --version`

5. **Build fails with "out of memory"**
   - Try building with fewer parallel jobs: `cargo build -j 2`
   - Close other applications to free up RAM

#### Verify Your Build

After building, you can verify the application works:

```bash
# Run the built executable directly
# Linux/macOS
./src-tauri/target/release/claudia

# Windows
./src-tauri/target/release/claudia.exe

# Windows 環境設定
為了確保 grep 和其他 Unix 工具在 Windows 環境下正常運作，需要設定以下環境變數：

## 必要的環境變數設定
1. **SHELL** 環境變數：
   ```
   SHELL=C:\Program Files\Git\bin\bash.exe
   ```

2. **PATH** 環境變數（確保包含 Git 工具路徑）：
   ```
   PATH=C:\Program Files\Git\bin;%PATH%
   ```

## 設定步驟
1. 開啟「系統內容」→「進階系統設定」→「環境變數」
2. 在「系統變數」或「使用者變數」中新增或編輯以下變數：
   - 變數名稱：`SHELL`
   - 變數值：`C:\Program Files\Git\bin\bash.exe`
3. 確保 PATH 中包含 Git 的 bin 目錄
4. 重新啟動應用程式以載入新的環境變數

## 故障排除
如果 grep 功能仍然無法正常運作，請檢查：
- Git for Windows 是否正確安裝
- SHELL 環境變數路徑是否正確指向 bash.exe
- 應用程式是否在設定環境變數後重新啟動
```

### Build Artifacts

The build process creates several artifacts:

- **Executable**: The main Claudia application
- **Installers** (when using `tauri build`):
  - `.deb` package (Linux)
  - `.AppImage` (Linux)
  - `.dmg` installer (macOS)
  - `.msi` installer (Windows)
  - `.exe` installer (Windows)

All artifacts are located in `src-tauri/target/release/bundle/`.

## 🛠️ Development

### Tech Stack

- **Frontend**: React 18 + TypeScript + Vite 6
- **Backend**: Rust with Tauri 2
- **UI Framework**: Tailwind CSS v4 + shadcn/ui
- **Database**: SQLite (via rusqlite)
- **Package Manager**: Bun

### Project Structure

```
claudia/
├── src/                   # React frontend
│   ├── components/        # UI components
│   ├── lib/               # API client & utilities
│   └── assets/            # Static assets
├── src-tauri/             # Rust backend
│   ├── src/
│   │   ├── commands/      # Tauri command handlers
│   │   ├── checkpoint/    # Timeline management
│   │   └── process/       # Process management
│   └── tests/             # Rust test suite
└── public/                # Public assets
```

### Development Commands

```bash
# Start development server
bun run tauri dev

# Run frontend only
bun run dev

# Type checking
bunx tsc --noEmit

# Run Rust tests
cd src-tauri && cargo test

# Format code
cd src-tauri && cargo fmt
```

## 🔒 Security

Claudia prioritizes your privacy and security:

1. **Process Isolation**: Agents run in separate processes
2. **Permission Control**: Configure file and network access per agent
3. **Local Storage**: All data stays on your machine
4. **No Telemetry**: No data collection or tracking
5. **Open Source**: Full transparency through open source code

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

### Areas for Contribution

- 🐛 Bug fixes and improvements
- ✨ New features and enhancements
- 📚 Documentation improvements
- 🎨 UI/UX enhancements
- 🧪 Test coverage
- 🌐 Internationalization

## 📄 License

This project is licensed under the AGPL License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Tauri](https://tauri.app/) - The secure framework for building desktop apps
- [Claude](https://claude.ai) by Anthropic

---

<div align="center">
  <p>
    <strong>Made with ❤️ by the <a href="https://asterisk.so/">Asterisk</a></strong>
  </p>
  <p>
    <a href="https://github.com/getAsterisk/claudia/issues">Report Bug</a>
    ·
    <a href="https://github.com/getAsterisk/claudia/issues">Request Feature</a>
  </p>
</div>


## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=getAsterisk/claudia&type=Date)](https://www.star-history.com/#getAsterisk/claudia&Date)
