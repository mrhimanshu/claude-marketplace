---
description: Analyze test coverage gaps and suggest missing test cases
disable-model-invocation: true
---

Analyze the selected code or module and identify what's NOT covered by existing tests. For each gap, suggest specific test cases.

**Analysis approach:**
1. Read the source code to understand all code paths
2. Read existing tests to see what's already covered
3. Identify untested paths, branches, and edge cases

**Report format:**

### Coverage Gaps Found

For each gap:
- **Location**: file:line — function/method name
- **What's missing**: Description of the untested path
- **Risk level**: High / Medium / Low
- **Suggested test**:
  ```
  test("should handle X when Y", () => {
    // test code
  })
  ```

### Summary
- Total functions/methods analyzed
- Estimated paths covered vs uncovered
- Priority order for writing missing tests

Focus on high-risk gaps first: error handling, security-sensitive paths, and complex branching logic.
