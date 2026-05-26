# .github

This repository holds org-level default configuration for the
[vergils-nemesis](https://github.com/vergils-nemesis) GitHub
organization — the adversarial testing counterpart to
[VERGIL](https://github.com/vergil-project).

## Table of Contents

- [What lives here](#what-lives-here)
- [How inheritance works](#how-inheritance-works)
- [The `.github/.github/` nesting](#the-githubgithub-nesting)
- [Related](#related)

## What lives here

| Path | Purpose |
|---|---|
| `profile/README.md` | Org profile page — renders on the [vergils-nemesis landing page](https://github.com/vergils-nemesis) |
| `profile/Mimir-Banner.png` | Org profile banner image |
| `CONTRIBUTING.md` | Contributor guidelines |
| `.github/workflows/ci.yml` | CI for this repo |

## How inheritance works

GitHub's `.github` profile repository provides org-level defaults.
Any repository in the org that does not have its own copy of a file
inherits the org default.

**Standalone files** (CONTRIBUTING.md, SECURITY.md, CODE_OF_CONDUCT.md,
SUPPORT.md, pull_request_template.md) inherit independently on a
per-file basis. A repo can override one without affecting the others.

**Template directories** (ISSUE_TEMPLATE/) inherit on a per-directory
basis — all or nothing. If a repo has any file in its own
`.github/ISSUE_TEMPLATE/` directory, it gets none of the org defaults
for that directory.

**Files that do not inherit**: LICENSE (each repo must have its own),
`.claude/`, `CLAUDE.md`, `vergil.toml`, and CI workflows.

## The `.github/.github/` nesting

This repo's own CI workflow lives at `.github/workflows/ci.yml`. The
outer `.github` is the repo name; the inner `.github/` is the standard
location for a repo's own workflows. This nesting is how GitHub
handles the `.github` repo having its own CI — it is correct, not a
mistake.

## Related

- [Org profile README](profile/README.md)
- [Contributing guidelines](CONTRIBUTING.md)
- [VERGIL project](https://github.com/vergil-project)
