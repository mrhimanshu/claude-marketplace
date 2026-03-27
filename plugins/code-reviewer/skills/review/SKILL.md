---
description: Review code for bugs, security issues, performance, and best practices
disable-model-invocation: true
---

Review the selected code or recent changes thoroughly. Analyze for:

**Bugs & Edge Cases**
- Null/undefined references, off-by-one errors, race conditions
- Unhandled error paths and missing input validation
- Logic errors and incorrect assumptions

Thanks

**Security Concerns**
- Injection vulnerabilities (SQL, XSS, command injection)
- Authentication/authorization gaps
- Sensitive data exposure or insecure defaults

**Performance Issues**
- Unnecessary re-renders, N+1 queries, memory leaks
- Missing memoization or caching opportunities
- Inefficient algorithms or data structures

**Code Quality**
- Readability and naming conventions
- DRY violations and unnecessary complexity
- Missing or misleading comments

Format your review as:
1. **Critical** — must fix before merge
2. **Warning** — should fix, potential issues
3. **Suggestion** — nice to have improvements

Be concise and actionable. Reference specific line numbers.
