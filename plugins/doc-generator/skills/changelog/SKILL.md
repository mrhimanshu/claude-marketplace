---
description: Generate a changelog from git history following Keep a Changelog format
disable-model-invocation: true
---

Analyze the git log and generate a changelog entry following the Keep a Changelog format (https://keepachangelog.com).

Group changes into:
- **Added** — new features
- **Changed** — changes to existing functionality
- **Deprecated** — features that will be removed
- **Removed** — features that were removed
- **Fixed** — bug fixes
- **Security** — vulnerability fixes

Rules:
- Read git log since the last tag or a reasonable range
- Write entries for humans, not machines
- Each entry should be a complete sentence
- Most recent changes first
- Include date in YYYY-MM-DD format
- Link to relevant PRs or issues if found in commit messages

Output format:
```markdown
## [version] - YYYY-MM-DD

### Added
- Description of new feature

### Fixed
- Description of bug fix
```

If an existing CHANGELOG.md exists, generate only the new section to prepend.
