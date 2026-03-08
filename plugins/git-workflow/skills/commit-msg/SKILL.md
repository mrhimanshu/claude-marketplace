---
description: Generate a conventional commit message from staged changes
disable-model-invocation: true
---

Look at the currently staged changes (git diff --cached) and generate a commit message following the Conventional Commits specification:

Format: `<type>(<scope>): <description>`

Types:
- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation changes
- **style**: Formatting, missing semicolons, etc.
- **refactor**: Code restructuring without behavior change
- **perf**: Performance improvements
- **test**: Adding or fixing tests
- **chore**: Build process, dependencies, tooling

Rules:
- Subject line under 72 characters
- Use imperative mood ("add" not "added")
- No period at the end of the subject
- Add body if changes need explanation
- Reference issue numbers if apparent from code

Provide 2-3 options ranked by quality. Show the best one first.
