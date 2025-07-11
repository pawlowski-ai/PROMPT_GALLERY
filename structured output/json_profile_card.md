
## Prompt
```
Generate a valid JSON object with the following structure:

{
  "full_name": string (max 60 chars),
  "age": integer,
  "email": string,
  "interests": array of strings (at least 3),
  "premium_user": boolean
}

Do not add any explanation. Only return a valid JSON object.
```
---
## Description
- Tests the model’s ability to produce a parsable and correctly typed JSON object with:
- Mixed value types
- A length constraint (max 60 chars)
- Array with minimum length
- Boolean handling
- It also tests whether the model can avoid natural language leakage and maintain key order.
---

### Expected Output
A clean, valid JSON object. Parsable with json.loads(), with correct types and field presence.

--- 
### Failure Patterns
- Non-parsable JSON (quotes, commas, brackets)

- Comments, natural language, or markdown wrappers

- Wrong types (e.g. age as string, boolean as “Yes”)

- Missing or excess keys

### Models Tested
GPT-4o (0613), Claude 3 Opus, Grok-3

### Notes
All models produced valid JSON in most trials. GPT-4o and Claude followed constraints well. Grok sometimes appended explanatory text after JSON. Claude occasionally re-ordered keys unless explicitly told to preserve order.

