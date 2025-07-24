---
"openapi-zod-client": minor
---

Add uniqueItems validation support for OpenAPI array schemas

- Arrays with `uniqueItems: true` now generate proper Zod validation with deep equality checking
- Uses fast-deep-equal library for efficient duplicate detection with early break optimization  
- Array validations (min, max, uniqueItems) are now applied at schema definition level for better semantics
- Maintains compatibility with existing functionality and proper dependency tracking
