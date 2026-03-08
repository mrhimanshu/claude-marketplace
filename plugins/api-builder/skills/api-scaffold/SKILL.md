---
description: Scaffold a REST API endpoint with routes, controllers, validation, and tests
disable-model-invocation: true
---

Scaffold a complete REST API endpoint. Detect the framework from the project (Express, FastAPI, Gin, Rails, etc.) and generate files following existing patterns.

**What to generate:**

1. **Route definition** — RESTful route (GET, POST, PUT, DELETE)
2. **Controller/Handler** — Request handling with proper error responses
3. **Input validation** — Schema validation for request body/params
4. **Database layer** — Model/migration if a database is detected
5. **Tests** — Unit tests for the endpoint
6. **Types** — TypeScript types / Pydantic models / Go structs as appropriate

**Conventions to follow:**
- Match the project's existing file structure and naming
- Use the project's existing patterns for error handling, auth, middleware
- Follow RESTful conventions (proper status codes, resource naming)
- Include proper HTTP status codes (200, 201, 400, 404, 500)
- Add input validation with meaningful error messages

**Usage:**
Tell me what resource/endpoint you need, e.g.:
- "Create a users endpoint with CRUD operations"
- "Add a POST /api/webhooks endpoint"
- "Scaffold a products API with search and pagination"
