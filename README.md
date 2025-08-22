🎨📊 Commit Grid Drawer Example
Welcome to the Commit Grid Drawer Example repository! This is a dedicated space to showcase the capabilities of the Commit Grid Drawer CLI tool. Here you'll find a live example of how the tool works and how it can be used to "draw" on your GitHub contribution graph.

This repository serves as a demonstration and will be automatically updated with daily commits orchestrated by the tool.

🚀 About Commit Grid Drawer
Commit Grid Drawer is a cross-platform CLI tool that automates daily commits to GitHub to "draw" custom patterns on your contribution graph. It offers a modern TUI (Text User Interface) for easy setup, flexible scheduling, and multiple strategies for commit intensity.

✨ Key Features
Automated Daily Commits: Effortlessly maintain a consistent contribution streak.

Pattern Drawing: Create unique designs on your contribution graph using fixed, random, or custom CSV-based patterns.

Interactive Setup: A friendly TUI guides you through configuring your repository, user, timezone, and schedule.

Cross-platform: Works seamlessly on Linux (using cron) and macOS (using launchd).

Configurable Intensity: Adjust the number of commits per day to suit your needs.

Lightweight: Built with Go, it's a single, static binary with no external dependencies or daemons.

🔗 Get the Tool
Ready to start drawing on your own contribution graph? You can find the main repository and the latest releases of the tool here:

Commit Grid Drawer on GitHub

⚙️ How It Works (This Repo)
This repository is configured to run the commit-grid tool daily. The configuration is stored in a .yaml file, and a scheduler (like cron on Linux) triggers the tool once a day.

Build and Setup
The commit-grid binary is built and configured to commit to this repository. The builds/ directory contains the Linux binary.

Bash

# Clone the main repository to build the binary
git clone https://github.com/laskydev/commit-grid-drawer.git
cd commit-grid-drawer

# Build the binary
go build -o commit-grid .
Configuration
The tool's configuration is managed through a YAML file. For this demo, the settings are configured to run with a specific pattern or intensity, which you can see in the config.yaml file (if provided) or by running the commit-grid config get command.

Scheduling
On Linux, the scheduler is a cron job that runs the command:

Bash

0 10 * * * /path/to/binary/commit-grid run >> ~/.local/state/commit-grid-draw/commit-grid.log 2>&1
This ensures the tool executes automatically every day at the specified time to generate the commits.
