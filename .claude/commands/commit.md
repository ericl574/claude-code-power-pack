---
description: Stage, group, and write clean Conventional Commits from your working changes
allowed-tools: Bash(git status:*), Bash(git diff:*), Bash(git add:*), Bash(git commit:*), Bash(git log:*)
---

You are creating high-quality git commits from the current working tree.

## Steps

1. Run `git status` and `git diff` (staged and unstaged) to understand every change.
2. Group the changes into the **smallest set of logically-coherent commits**. Do not lump unrelated changes together. A bug fix, a new feature, and a docs tweak are three commits, not one.
3. For each group:
   - Stage exactly the files/hunks that belong to it.
   - Write a [Conventional Commits](https://www.conventionalcommits.org) message: `type(scope): summary` where type is one of feat, fix, docs, style, refactor, perf, test, build, ci, chore.
   - Keep the summary under 72 chars, imperative mood ("add" not "added").
   - Add a body only when the *why* isn't obvious from the diff.
4. Show me the planned commits **before** running them. Wait for my confirmation unless I said "just commit".
5. Never commit secrets, `.env` files, or large binaries — flag them instead.

$ARGUMENTS
