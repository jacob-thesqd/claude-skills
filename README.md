# Claude Code Skills — The Squad

Shared Claude Code skills for the Squad team.

## Available Skills

| Skill | Command | Description |
|-------|---------|-------------|
| **Squad App Audit** | `/squad-app-audit` | Comprehensive Next.js project audit across 7 categories (A–F grading) |

## Installation

### One-line install (all skills)

```bash
curl -sL https://raw.githubusercontent.com/jacob-thesqd/claude-skills/main/install.sh | bash
```

### Manual install (single skill)

```bash
mkdir -p ~/.claude/commands
curl -o ~/.claude/commands/squad-app-audit.md https://raw.githubusercontent.com/jacob-thesqd/claude-skills/main/skills/squad-app-audit.md
```

## Usage

Once installed, open Claude Code in any project and run:

```
/squad-app-audit
```

Claude will:
1. Detect your project structure (App Router, Pages Router, monorepo)
2. Count files and estimate audit time
3. Ask for confirmation before proceeding
4. Audit across 7 categories and grade each A–F
5. Save a detailed report to `AUDIT_REPORT.md` and print it

## Updating

Re-run the install script to get the latest versions:

```bash
curl -sL https://raw.githubusercontent.com/jacob-thesqd/claude-skills/main/install.sh | bash
```

## Adding New Skills

1. Create a `.md` file in the `skills/` directory
2. Add the skill name to `install.sh`
3. Update this README
4. Push to `main`
