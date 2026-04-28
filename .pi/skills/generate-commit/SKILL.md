---
name: generate-commit
description: Generates a conventional commit message by analyzing code changes. Use when the user asks to "create a commit", "generate a commit message", or wants to commit their recent code changes.
---
# Skill: Generate Commit Message

## Instructions

When asked to generate a commit message, follow these steps:

1.  **Gather Context:**
    *   Check for staged changes: `git diff --cached`
    *   Check for unstaged changes: `git diff`
    *   Check for untracked files: `git status -u`

2.  **Analyze Changes:**
    *   Review the collected diffs and file statuses.
    *   Identify the primary intent of the changes (e.g., new feature, bug fix, refactor, documentation, chore).
    *   Identify the main parts of the codebase affected (e.g., `account` app, `bookmarks` settings).

3.  **Draft Commit Message:**
    *   Construct a commit message following the Conventional Commits specification.
    *   **Header:** `type(scope): summary`
        *   `type`: feat, fix, chore, docs, style, refactor, test, etc.
        *   `scope`: The module or area of the project that was changed (e.g., `account`, `ci`, `deps`).
        *   `summary`: A concise, imperative-tense description of the change.
    *   **Body (optional):** A more detailed explanation of the changes, including the "why" and "what."

4.  **Confirm and Commit:**
    *   Present the full drafted message to the user for approval.
    *   Ask if they want to use the full message, only the header, or make modifications.
    *   Once approved, add the relevant files to staging and execute the `git commit` command.
