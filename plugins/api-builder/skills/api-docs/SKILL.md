---
description: Generate OpenAPI/Swagger documentation from existing API code
disable-model-invocation: true
---

Analyze the existing API routes and generate OpenAPI 3.0 documentation.

**What to extract:**
- All API endpoints (path, method, description)
- Request parameters (path, query, header, cookie)
- Request body schemas with examples
- Response schemas for all status codes
- Authentication requirements
- Rate limiting info (if present)

**Output format — OpenAPI 3.0 YAML:**

```yaml
openapi: 3.0.3
info:
  title: API Name
  version: 1.0.0
paths:
  /resource:
    get:
      summary: List resources
      parameters: [...]
      responses:
        '200':
          description: Success
          content:
            application/json:
              schema: {...}
              example: {...}
```

**Rules:**
- Include realistic example values
- Document error responses (400, 401, 403, 404, 500)
- Group endpoints by tags
- Add descriptions that explain business logic, not just "gets a thing"
- If an existing OpenAPI spec exists, update it rather than replacing it
