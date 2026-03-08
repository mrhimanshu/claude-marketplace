---
description: Generate comprehensive unit and integration tests for selected code
disable-model-invocation: true
---

Generate thorough tests for the selected code. Auto-detect the language and testing framework from the project (Jest, Pytest, Go testing, RSpec, etc.).

**Test categories to generate:**

1. **Happy path** — normal expected behavior
2. **Edge cases** — boundary values, empty inputs, max values
3. **Error cases** — invalid inputs, missing data, network failures
4. **Integration** — interaction between components (if applicable)

**Test quality rules:**
- Each test should test ONE thing
- Use descriptive test names that explain the expected behavior
- Follow AAA pattern: Arrange, Act, Assert
- Mock external dependencies (APIs, databases, file system)
- Include setup/teardown where needed
- Avoid testing implementation details — test behavior

**Output:**
- Complete, runnable test file
- Match the project's existing test patterns and conventions
- Include any needed imports and test fixtures
- Add brief comments for non-obvious test cases

Detect the test framework from the project. If unclear, ask which framework to use.
