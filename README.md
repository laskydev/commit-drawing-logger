# Commit Grid Drawer Logger 🎨📊

A demonstration repository showcasing the **Commit Grid Drawer** tool in action - a cross-platform CLI tool that automates daily commits to GitHub to "draw" custom patterns on your contribution graph.

## 🚀 What is Commit Grid Drawer?

Commit Grid Drawer is a powerful automation tool that allows you to:

- ✨ Create artistic patterns on your GitHub contribution graph
- 🤖 Automate daily commits with flexible scheduling
- 🎯 Configure custom intensity strategies (fixed, random, or pattern-based)
- 🖥️ Work seamlessly across Linux and macOS platforms
- 📊 Use CSV files to define complex drawing patterns

## 📁 This Repository

This logger repository serves as a **live demonstration** of Commit Grid Drawer in action. Here you can:

- See real commit patterns being generated automatically
- Explore the `data/grid.csv` file to understand how patterns are tracked
- View commit history to see the tool's daily automation
- Access pre-built binaries for easy installation

## 🔗 Get Started

Ready to create your own contribution graph art? Head over to the main project:

**👉 [Visit the Commit Grid Drawer Repository](https://github.com/laskydev/commit-grid-drawer)**

## 📦 Quick Installation

### Linux (Ubuntu)
```bash
# Download the latest Linux binary
wget https://github.com/[username]/commit-grid-drawer-logger/releases/latest/download/commit-grid-linux
chmod +x commit-grid-linux
sudo mv commit-grid-linux /usr/local/bin/commit-grid

# Run the interactive setup
commit-grid init
```

### macOS
```bash
# macOS binary coming soon!
# For now, build from source at the main repository
```

## 🎨 Features Overview

- **Interactive Setup**: Modern TUI onboarding experience
- **Cross-Platform Scheduling**: Automatic cron (Linux) and launchd (macOS) integration
- **Multiple Strategies**:
  - `fixed` - Same number of commits daily
  - `random` - Random intensity within range
  - `pattern` - CSV-based custom patterns
- **Timezone Support**: Configure your local timezone for accurate scheduling
- **Safe & Portable**: Self-contained Go binary with comprehensive logging

## 📊 Example Patterns

This repository demonstrates various commit patterns:

- Daily consistent commits (fixed strategy)
- Weekly patterns with varying intensity
- Custom designs loaded from CSV files

## 🛠️ Configuration

The tool uses a simple YAML configuration:

```yaml
repo_path: "./drawing"
git_user: "your-username"
git_email: "your-email@example.com"
timezone: "America/Monterrey"
hour_24: 10
minute: 0
intensity_strategy: "fixed"
intensity_value: 1
```

## 📈 Monitoring & Logs

All activity is logged for transparency:

- **Linux**: `~/.local/state/commit-grid-draw/commit-grid.log`
- **macOS**: `~/Library/Logs/commit-grid.log`

## 🤝 Contributing

Found a bug or have a feature request? Please visit the main repository:

**[Commit Grid Drawer Issues](https://github.com/laskydev/commit-grid-drawer/issues)**

## ⚠️ Responsible Use

This tool is designed for creative expression and learning purposes. Please use it responsibly:

- Avoid excessive commit spam
- Respect GitHub's terms of service
- Keep patterns fun and meaningful

## 📄 License

This project is licensed under the same terms as the main Commit Grid Drawer tool.

---

**🔗 Main Project**: [github.com/laskydev/commit-grid-drawer](https://github.com/laskydev/commit-grid-drawer)

Made with ❤️ for the GitHub community
