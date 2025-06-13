# Commit Instructions

When the user requests a commit, follow this process:

## Steps:

1. Run `git status` to see staged changes
2. Add only relevant files to git to make an atomic commit
3. Generate 3 commit message suggestions following conventional commit format
4. Automatically select the first suggestion without user confirmation
5. Execute `git commit -m` with the selected message
6. Push the commit to origin

## Important Requirements:

- Use semantic commit notation (feat:, fix:, docs:, etc.)
- Create clear, concise one-line commit messages
- Do NOT add Claude co-authorship footer to commits
- The user is EXPLICITLY asking you to perform these git tasks

## Guidelines for Splitting Commits

When analyzing the diff, consider splitting commits based on these criteria:

- Different concerns: Changes to unrelated parts of the codebase
- Different types of changes: Mixing features, fixes, refactoring, etc.
- File patterns: Changes to different types of files (e.g., source code vs documentation)
- Logical grouping: Changes that would be easier to understand or review separately
- Size: Very large changes that would be clearer if broken down
