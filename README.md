# Claude Community Marketplace

A distributed plugin marketplace for [Claude Code](https://claude.com/claude-code) with 6 plugins and 12 slash commands for developer productivity.

## Plugins

| Plugin | Commands | Description |
|--------|----------|-------------|
| **code-reviewer** | `/review`, `/security-audit` | AI-powered code review and OWASP security auditing |
| **git-workflow** | `/pr-summary`, `/commit-msg` | Generate PR summaries and conventional commit messages |
| **doc-generator** | `/docs`, `/changelog` | Generate documentation and Keep a Changelog entries |
| **test-helper** | `/test-gen`, `/coverage` | Generate tests and analyze coverage gaps |
| **refactor-tools** | `/refactor`, `/simplify` | Intelligent refactoring and code simplification |
| **api-builder** | `/api-scaffold`, `/api-docs` | Scaffold REST endpoints and generate OpenAPI specs |

## Install

Add this marketplace to Claude Code:

```shell
/plugin marketplace add <your-github-username>/claude-marketplace
```

Install individual plugins:

```shell
/plugin install code-reviewer@claude-community-marketplace
/plugin install git-workflow@claude-community-marketplace
/plugin install doc-generator@claude-community-marketplace
/plugin install test-helper@claude-community-marketplace
/plugin install refactor-tools@claude-community-marketplace
/plugin install api-builder@claude-community-marketplace
```

## Update

```shell
/plugin marketplace update
```

## Structure

```
.claude-plugin/
└── marketplace.json          # Marketplace catalog

plugins/
├── code-reviewer/            # /review, /security-audit
├── git-workflow/             # /pr-summary, /commit-msg
├── doc-generator/            # /docs, /changelog
├── test-helper/              # /test-gen, /coverage
├── refactor-tools/           # /refactor, /simplify
└── api-builder/              # /api-scaffold, /api-docs
```

## License

MIT
