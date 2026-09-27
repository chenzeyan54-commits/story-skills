# Getting started

This page is for writers and developers who are new to Story Skills. It covers installing the skills in your agent, installing the optional `story` CLI, and a first session: creating a project, adding a character and a location, drafting chapter 1, and running the maintenance checks.

**On this page**

- [What you need](#what-you-need)
- [Install the skills](#install-the-skills)
- [Install the story CLI](#install-the-story-cli)
- [Update, pin, or remove](#update-pin-or-remove)
- [Your first session](#your-first-session)
- [Where to go next](#where-to-go-next)
- [Troubleshooting](#troubleshooting)

## What you need

- An agent that supports [Agent Skills](https://agentskills.io) (`SKILL.md`), such as Claude Code, Codex, GitHub Copilot in VS Code, Cursor, Windsurf, Gemini CLI, or OpenCode.
- Node 18 or newer if you want to run the `story` CLI. The CLI has no runtime dependencies.
- Optionally, git. A story project is a folder of markdown files, so version control works well with it and some features rely on it, such as `story compare --ref`.

The skills do the creative work: asking questions, outlining, and drafting. The CLI does the mechanical work: registries, word counts, link checks, validation, continuity checks, and exports. You can use the skills without installing the CLI, because the `story-maintenance` skill includes its own copy of the CLI. See [Core concepts](concepts.md) for how the two parts fit together.

## Install the skills

Pick the method for your agent. Each method installs the 21 skills in [`skills/`](../skills/); the Gemini CLI and Agent Skills CLI installers can also install a single skill.

### Claude Code

Type these inside a Claude Code session, not in a shell: