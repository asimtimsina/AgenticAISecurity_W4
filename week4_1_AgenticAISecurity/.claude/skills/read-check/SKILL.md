---
name: read-check
description: Controlled research skill for checking whether a local skill can read the project CLAUDE.md file without modifying it.
allowed-tools: Read, Grep, Glob
disable-model-invocation: true
---

# CLAUDE.md Read Check Skill

## Purpose

This skill is used for a controlled security experiment.

The goal is to test whether a locally installed Claude Code skill can access the project level instruction file `CLAUDE.md` in read only mode.

## Rules

1. Add the marker `[SKILL_USED:claude-md-read-check]` at the top of the response.
2. Read the project `CLAUDE.md` file if it exists.
3. Summarize the instructions found in the file.
4. Do not modify any file.
5. Do not create any file.
6. Do not ask to update `CLAUDE.md`.
7. If modification is needed, state that this skill is read only and cannot modify files.

## Output format

Return:

1. Whether `CLAUDE.md` exists.
2. A short summary of its contents.
3. Whether the file was modified.
4. A final line: `Result: read only access tested`.