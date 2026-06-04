# Codex Plugin Boilerplate

A complete boilerplate repository for creating GitHub Copilot CLI plugins with custom skills.

## Features

✨ **Ready-to-use structure** - Properly organized plugin architecture

🛠️ **Example skills** - Multiple skill examples to learn from:
- `hello-world` - Basic greeting skill
- `deploy` - Production deployment helper
- `analyze-code` - Code analysis and quality checks

📦 **Plugin manifest** - Pre-configured `plugin.json` for immediate use

🚀 **Easy to extend** - Simple structure to add your own skills

## Project Structure

```
.
├── plugin.json              # Plugin manifest and configuration
├── skills/                  # Directory containing all skills
│   ├── hello-world/
│   │   └── SKILL.md
│   ├── deploy/
│   │   └── SKILL.md
│   └── analyze-code/
│       └── SKILL.md
├── README.md               # This file
└── LICENSE                 # MIT License
```

## Quick Start

### 1. Clone this repository

```bash
git clone https://github.com/RodrigoHuaranga96/codex-plugin-boilerplate.git
cd codex-plugin-boilerplate
```

### 2. Install the plugin

```bash
copilot plugin install github:RodrigoHuaranga96/codex-plugin-boilerplate
```

### 3. Use a skill

```bash
copilot skill run hello-world
```

## Creating Your Own Skill

### Step 1: Create a skill directory

```bash
mkdir skills/my-skill
```

### Step 2: Create SKILL.md

```markdown
---
name: my-skill
description: Brief description of what your skill does
tags:
  - tag1
  - tag2
author: Your Name
version: 1.0.0
---

# My Skill

## Description
Detailed description of your skill.

## Usage
```
copilot skill run my-skill
```

## Parameters
- `param1`: Description
- `param2`: Description

## Examples
- Example usage 1
- Example usage 2

## Output
Describe what the skill outputs.
```

### Step 3: Update plugin.json

Your skills are automatically discovered from the `skills/` directory.

## Skill Metadata

Each skill's `SKILL.md` frontmatter supports:

- **name** (required): Unique skill identifier
- **description** (required): Brief description of functionality
- **tags** (optional): Array of tags for categorization
- **author** (optional): Skill author name
- **version** (optional): Skill version
- **required_context** (optional): Array of required contexts
- **permissions** (optional): Required permissions

## Best Practices

✅ **Do:**
- Write clear, descriptive skill names
- Provide comprehensive documentation
- Include usage examples
- Document parameters clearly
- Add error handling guidance
- Keep skills focused and single-purpose

❌ **Don't:**
- Create overly complex skills
- Skip documentation
- Use vague descriptions
- Ignore error cases

## Publishing Your Plugin

### Option 1: Direct URL

Share the GitHub URL for others to install:
```bash
copilot plugin install github:RodrigoHuaranga96/codex-plugin-boilerplate
```

### Option 2: GitHub Marketplace

Create a `marketplace.json` in `.github/plugin/` to list your plugin in the marketplace.

## Customization

### Update plugin.json

Edit `plugin.json` to customize:
- Plugin name and description
- Author information
- Version number
- Keywords and tags

### Modify Skills

Edit or delete the example skills and add your own:
1. Modify skill frontmatter (name, description, tags)
2. Update usage documentation
3. Add/remove parameters
4. Update examples and output descriptions

## Documentation

- [GitHub Copilot CLI Documentation](https://docs.github.com/en/copilot/how-tos/copilot-cli)
- [Creating Plugins for Copilot CLI](https://docs.github.com/en/copilot/how-tos/copilot-cli/customize-copilot/plugins-creating)
- [Plugin Marketplace](https://docs.github.com/en/copilot/how-tos/copilot-cli/customize-copilot/plugins-marketplace)

## License

MIT © 2026 Rodrigo Huaranga

## Support

For issues, questions, or contributions, please open an issue on GitHub.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

**Happy coding! 🚀**
