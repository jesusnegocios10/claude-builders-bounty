# Changelog Generator

A simple bash script that generates a structured `CHANGELOG.md` from your project's git history.

## Setup (3 steps)

1. **Download the script:**
   ```bash
   curl -o changelog.sh https://raw.githubusercontent.com/YOUR_REPO/main/changelog.sh
   chmod +x changelog.sh
   ```

2. **Run in any git repo:**
   ```bash
   cd /path/to/your/repo
   bash /path/to/changelog.sh
   ```

3. **Check the output:**
   ```bash
   cat CHANGELOG.md
   ```

## Features

- Auto-categorizes commits into: `Added`, `Fixed`, `Changed`, `Removed`
- Works with semantic version tags (v1.0.0, v2.3.1, etc.)
- Falls back to chronological order when no tags exist
- Supports conventional commit prefixes (feat:, fix:, etc.)
- Generates clean Markdown output

## Usage

```bash
# Generate CHANGELOG.md in current directory
bash changelog.sh

# Generate to a specific file
bash changelog.sh docs/CHANGELOG.md
```

## Accepted Stack

- Bash
- Python
- Native Claude Code SKILL.md

## Tested On

- GitHub repositories with git tag history
- Works on Linux, macOS, and Windows (Git Bash / WSL)
