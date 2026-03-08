---
description: Simplify overly complex code — reduce nesting, remove abstractions, flatten logic
disable-model-invocation: true
---

Analyze the selected code and aggressively simplify it. The goal is fewer lines, less nesting, and less abstraction while keeping the same behavior.

**Simplification strategies:**
- Flatten deeply nested if/else chains with early returns
- Replace verbose patterns with language idioms (map/filter/reduce, list comprehensions, etc.)
- Inline trivial helper functions that are only called once
- Remove unnecessary abstractions and wrapper classes
- Simplify boolean expressions
- Replace complex state machines with simpler alternatives
- Use built-in library functions instead of hand-rolled logic
- Remove defensive coding that can't actually happen

**Rules:**
- Behavior must remain identical
- Prefer readability over cleverness
- Three lines of clear code > one line of clever code
- Don't simplify away necessary error handling
- Show before/after line counts

**Output:**
Apply the simplifications directly and provide a brief summary of what was simplified and why.
