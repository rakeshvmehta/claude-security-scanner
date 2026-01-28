# Claude Code Plugins

Shared plugins for Claude Code.

## Available Plugins

| Plugin | Description |
|--------|-------------|
| [security-scan](./security-scan) | Security review with stack-specific context, compliance tracking, and Slack integration |

## Installation

### Option 1: Add as Marketplace (Recommended for Teams)

Add this repo as a marketplace, then install plugins:

```bash
# Add the marketplace (one-time)
claude plugin marketplace add https://github.com/Zarna-AI/claude-plugins

# Install the plugin (project scope recommended)
claude plugin install security-scan --scope project
```

### Option 2: Local Development

Clone and use directly:

```bash
git clone https://github.com/Zarna-AI/claude-plugins.git
claude --plugin-dir /path/to/claude-plugins/security-scan
```

## For Team Members

One-time setup for new team members:

```bash
# Add the marketplace (one-time)
claude plugin marketplace add https://github.com/Zarna-AI/claude-plugins

# Install for this project only (recommended)
claude plugin install security-scan --scope project

# Or install for all projects
claude plugin install security-scan --scope user
```

Then:
1. Set required environment variables (see each plugin's README)
2. Run the plugin's setup command (e.g., `/security-setup`)

## Contributing

To add a new plugin:
1. Create a new directory with the plugin name
2. Follow the Claude Code plugin structure
3. Add to the table above
4. Submit a PR
