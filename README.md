# Solvex Skills

Claude Code Skills for Solvex team. Install via `npx skills`.

## Available Skills

| Skill | Description | Install |
|-------|-------------|---------|
| traffic-standards-kb | Chinese smart transportation standards knowledge base (GB/JT/T/GA) | `npx skills add solvex-top/solvex-skills@traffic-standards-kb -g -y` |

## Quick Start

### Prerequisites

- [Claude Code](https://claude.ai/code) installed
- `npx` available (comes with Node.js)

### Install a Skill

```bash
# Install globally (available in all projects)
npx skills add solvex-top/solvex-skills@traffic-standards-kb -g -y

# Install to current project only
npx skills add solvex-top/solvex-skills@traffic-standards-kb -y
```

### Configure API Key

For `traffic-standards-kb`, set the API key after installation:

```bash
# Option 1: Global settings (~/.claude/settings.json)
# Add to "env" section:
# "STANDARDS_API_KEY": "your-api-key"

# Option 2: Shell environment variable
export STANDARDS_API_KEY="your-api-key"
```

Get your API key from: https://top.solvexpert.top

### Manage Skills

```bash
npx skills list              # List installed skills
npx skills update            # Update all skills
npx skills remove <name>     # Remove a skill
```

## Skill Details

### traffic-standards-kb

Retrieve Chinese transportation standards (GB, JT/T, GA/T) via Solvex API for smart transportation solutions.

**Supported domains:** Signal control, parking, monitoring, data collection, tolling, smart highway, service area, public transit, V2X, MaaS, and emerging areas.

**Trigger:** Automatically activated when writing smart transportation solutions or technical proposals requiring industry standards citation.

See [skills/traffic-standards-kb/README.md](skills/traffic-standards-kb/README.md) for full documentation.

## Adding New Skills

1. Create a new directory under `skills/`
2. Add a `SKILL.md` with frontmatter (`name`, `description`)
3. Add any supporting files (reference docs, scripts, etc.)
4. Update this README's Available Skills table
5. Commit and push

## Repository Structure

```
solvex-skills/
├── README.md                           # This file
└── skills/
    └── traffic-standards-kb/
        ├── SKILL.md                    # Skill definition (trigger + usage)
        ├── api-reference.md            # Detailed API documentation
        └── README.md                   # Comprehensive usage guide
```
