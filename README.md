# Rootline Agent Skills

Agent skills for [Rootline](https://github.com/pablontiv/rootline) — a file-based database and constraint engine for structured documentation.

These skills teach AI agents how to validate, inspect, scaffold, and plan structured documentation projects powered by Rootline's `.stem` schema system.

## Prerequisites

Rootline CLI must be installed and available in your PATH.

**Install from GitHub Releases:**

```bash
# Download the latest release for your platform
# See https://github.com/pablontiv/rootline/releases
./install.sh
```

Or download manually from [Rootline Releases](https://github.com/pablontiv/rootline/releases).

## Installation

### Any AI Agent (skills.sh)

Works with Claude Code, Cursor, Gemini CLI, OpenCode, Augment, Copilot, and more:

```bash
npx skills add pablontiv/agent-marketplace
```

### Claude Code Plugin

Register this repository as a Claude Code marketplace:

```
/plugin marketplace add pablontiv/agent-marketplace
```

Then install the rootline-core plugin:

```
/plugin install rootline-core@rootline-agent-skills
```

## Available Skills

| Skill | Description | Compatible Agents |
|-------|-------------|-------------------|
| **rootline-validate** | Validate documents against `.stem` schemas. Checks frontmatter fields for required values, enum constraints, and structural rules. | All (skills.sh) |
| **rootline-describe** | Show the effective `.stem` schema for a directory. Displays fields, types, required status, enum values, and inheritance chain. | All (skills.sh) |
| **rootline-new-doc** | Scaffold new documents with correct frontmatter based on `.stem` schema. Uses auto-numbering for sequential IDs. | All (skills.sh) |
| **rootline-roadmap** | AI-native planning framework for project decomposition into epics, features, stories, and tasks with binary acceptance criteria. | All (skills.sh) |

## About Rootline

Rootline treats the filesystem as a database: directories are tables, files are records, metadata comes from YAML frontmatter, and structure is inherited via `.stem` files. Learn more at [github.com/pablontiv/rootline](https://github.com/pablontiv/rootline).
