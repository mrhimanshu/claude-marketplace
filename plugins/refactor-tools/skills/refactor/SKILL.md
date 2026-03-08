---
description: Analyze and refactor code for better structure, readability, and maintainability
disable-model-invocation: true
---

Analyze the selected code and suggest targeted refactorings. Apply the changes directly.

**Refactoring patterns to look for:**
- Extract method/function for repeated or complex logic
- Rename variables/functions for clarity
- Replace conditionals with polymorphism or strategy pattern
- Simplify nested conditionals with early returns/guard clauses
- Remove dead code and unused variables
- Break large functions into smaller, focused ones
- Replace magic numbers with named constants
- Consolidate duplicate code

**Rules:**
- Preserve ALL existing behavior — refactoring must not change functionality
- Make the smallest changes that improve the code
- Each refactoring should be independently valuable
- Explain WHY each change improves the code
- If tests exist, ensure they still pass after refactoring

**Output:**
1. List of refactorings applied with brief explanation
2. Apply the changes to the code
3. Note any refactorings you considered but skipped (and why)
