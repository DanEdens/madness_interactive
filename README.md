# Madness Interactive

A collection of project templates and interactive development tools for various programming languages and frameworks.

## Overview

This repository serves as a template hub for creating new projects with predefined structures, best practices, and development workflows. It supports multiple programming languages and frameworks, making it easy to start new projects with consistent organization and tooling.

# Human readable .cursorrules

env = windows cmd. wsl and powershell are available You can check for the availability of the commands in the environment at will
0. Use trunk-based development with feature branches. use gh cli as needed. Be detailed, I love traciability.
1. Work on the problem as asked here. Be careful not to backtrack on progress for existing methods.
2. Run available tests (e.g. 'cargo test') and iterate (word for new stuff that doesnt have to mess up other stuff)
3. Maintain a "Lessons Learned" section in readme.md
4. Update readme.md with progress after completing features
5. Git workflow rules:
   - Always append '| cat' to commands that might trigger a pager (git diff, git log, etc.)
   - Use --no-pager flag for git commands when possible
   - Keep commit messages single-line or use multiple -m flags
   - Include ticket/issue numbers in commit messages when applicable
   - Write detailed commit messages for future debugging reference
6. Command execution rules:
   - Avoid newlines in command strings
   - Use semicolons or && for multiple commands instead of newlines
   - Escape special characters in command strings
   - Set appropriate flags to prevent interactive prompts
7. Test failure triage process:
   - Analyze the root cause without immediately modifying the test
   - Identify which components or features are impacted
   - Assess the broader architectural implications
   - Prioritize preservation of existing functionality
   - Propose minimal, targeted fixes that maintain system integrity

Evaluation Criteria:
- Does the proposed fix preserve existing features?
- Is the change minimal and focused?
- Does it address the underlying architectural concern?
- Will it introduce new complexity or potential regressions?

Recommended Actions:
- Comment out problematic code instead of deleting
- Create feature flags for experimental changes
- Document the issue in "Lessons Learned"
- Discuss potential systemic improvements



## Project Languages

[X] Python
[X] Rust
[X] Powershell
[X] Lua
[X] OS
[ ] Go
[ ] C#
[ ] JavaScript
[ ] C++
[ ] Java
[ ] Ruby
[ ] PHP
[ ] TypeScript


## Project Structure

```
madness_interactive/
├── projects/
│   ├── python/
│   │   ├── ai_interface/
│   │   ├── mcp_server/
│   │   ├── EventGhost/
│   │   ├── simple-mqtt-server-agent/
│   │   ├── mqtt-get-var/
│   │   ├── local-ai/
│   │   ├── dvtTestKit/
│   │   ├── SeleniumPageUtilities/
│   │   ├── MqttLogger/
│   │   ├── LegoScry/
│   │   └── games/
│   ├── powershell/
│   │   └── WinSystemSnapshot/
│   ├── lua/
│   │   ├── hammerspoon/
│   │   └── LGS_script_template/
│   ├── rust/
│   │   ├── Tinker/
│   │   └── EventGhost-Rust/
│   ├── common/
│   └── OS/
├── templates/
│   ├── python/
│   ├── rust/
│   └── [future-languages]/
├── docs/
│   ├── python/
│   └── rust/
├── scripts/
│   ├── init_python_project.sh
│   └── init_rust_project.sh
├── theming/
├── prompts/
└── README.md
```

## Subprojects

### Python Projects

#### EventGhost
An advanced, yet easy-to-use extensible automation tool for Windows. Users can create macros entirely through the GUI to be triggered by events from any device, program or source with a corresponding plugin.

#### AI Interface & MCP Server
A modern AI-powered control system for EventGhost:
- **ai_interface**: Constructs and sends Events, Actions and Macros to EventGhost via XML
- **mcp_server**: Socket server that forwards commands from AI interface to EventGhost

#### MQTT Tools
- **simple-mqtt-server-agent**: Lightweight MQTT server with agent capabilities
- **mqtt-get-var**: Tool for retrieving variables via MQTT
- **MqttLogger**: Logging system built on MQTT protocol

#### Testing & Automation
- **dvtTestKit**: Device validation testing toolkit
- **SeleniumPageUtilities**: Helper utilities for Selenium page testing
- **LegoScry**: Computer vision tools for LEGO brick recognition
- **local-ai**: Local AI model integration tools

### Rust Projects

#### EventGhost-Rust
A modern, fast, and extensible reimplementation of EventGhost in Rust. Currently focusing on:
- Robust plugin system architecture
- Win32 API integration
- Core event system
- Plugin manifest format
- Dynamic library loading

#### Tinker
A Madness engineered browser built for tinkerers and test enthusiasts:
- MQTT-powered control mechanisms
- Universal Workbench API
- Built-in diagnostic dashboard
- Test blueprint management
- Session versioning and comparison
- Precision event engineering

### PowerShell Projects

#### WinSystemSnapshot
Tools for capturing and analyzing Windows system state:
- System configuration snapshots
- Change detection
- State comparison tools
- Automated reporting

### Lua Projects

#### Hammerspoon
Custom Hammerspoon configurations and extensions:
- Window management
- Application control
- System automation
- Custom spoons

#### LGS Script Template
Logitech Gaming Software script templates:
- Macro definitions
- Profile management
- Device configurations
- Event handlers

### Common & OS Projects
Shared utilities and OS-specific tools used across projects:
- Cross-project utilities
- System integration helpers
- Platform-specific implementations
- Shared configurations

## Features

- 📁 Organized template structure for multiple languages
- 🔧 Project initialization scripts
- 📝 Comprehensive documentation templates
- 🧪 Testing frameworks setup
- 🚀 CI/CD configurations
- 📊 Project management tools

## Getting Started

### Creating a New Project

1. Choose a language template:
   ```bash
   # For Python projects
   ./scripts/init_python_project.sh [template-name] [project-name]

   # For Rust projects
   ./scripts/init_rust_project.sh [template-name] [project-name]
   ```

2. Follow the template-specific README for additional setup steps

## Contributing

We welcome contributions! Whether it's:
- Adding new language templates
- Improving existing templates
- Fixing bugs
- Enhancing documentation

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## Template Standards

Each template should include:
- README.md with clear instructions
- Documentation templates
- Testing setup
- Development environment configuration
- CI/CD setup where applicable
- .gitignore and other necessary configurations

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Lessons Learned

See [LESSONS_LEARNED.md](LESSONS_LEARNED.md) for insights and best practices gathered during development.
