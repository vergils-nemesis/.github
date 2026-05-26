# CLAUDE.md

## Project Overview

Organization profile and community health files for
[vergils-nemesis](https://github.com/vergils-nemesis) — the
adversarial testing counterpart to the
[VERGIL](https://github.com/vergil-project) methodology.

This is a documentation-only repository. It contains the org
profile README, contributing guide, and community health files.
No code, no CI, no releases.

## Shell command policy

Use `vrg-git` instead of `git` for all git operations. Use `vrg-gh`
instead of `gh` for all GitHub CLI operations. These wrappers enforce
subcommand allowlists, flag deny lists, credential selection, and
audit logging.

Raw `git` and `gh` are denied by the permission model. If a command
is not available through the wrappers, explain the situation to the
human who can run it directly via `! <command>` in the prompt.

## Development Commands

### Validation

```bash
vrg-docker-run -- uv run vrg-validate
```

### Commits

Use `vrg-commit` for all commits. Raw `git commit` is blocked by
the pre-commit hook.

### Pull Requests

Use `vrg-submit-pr` for all pull requests.

## File Layout

```text
.claude/settings.json    — Claude Code permissions and plugin config
.claude/hooks/guard.sh   — Claude Code PreToolUse hook guard
profile/README.md        — org profile (rendered on github.com/vergils-nemesis)
profile/Mimir-Banner.png — org profile banner image
CLAUDE.md                — this file
CONTRIBUTING.md          — contributing guide
README.md                — repo description
vergil.toml              — VERGIL tooling configuration
```
