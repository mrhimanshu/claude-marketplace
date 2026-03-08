---
description: Generate a comprehensive PR summary from staged/committed changes
disable-model-invocation: true
---

Analyze the current git diff (staged and unstaged changes) or the commits on the current branch compared to main/master. Generate a pull request summary with:

## Summary
- 2-4 bullet points describing what changed and why
- Focus on the "why" not just the "what"

## Changes
- Group related changes by area (e.g., API, UI, Database, Config)
- List key files modified with brief descriptions

## Testing
- Suggest what should be tested
- Note any areas of risk

## Breaking Changes
- List any breaking changes or migration steps needed
- Note backwards-compatibility concerns

Output the summary in markdown format ready to paste into a PR description.
