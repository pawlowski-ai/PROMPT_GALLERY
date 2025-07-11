# 📦 Structured Output Prompts

**Purpose**  
This folder contains prompts that force or evaluate the generation of structured outputs such as JSON, XML, or tables. Structuring output is essential when integrating LLMs into pipelines, APIs, databases, or multi-agent systems that require machine-readable responses.

**Why this matters**  
LLMs are not guaranteed to follow schemas. Even simple requests like "respond in JSON" often fail at:
- Opening/closing brackets
- Unexpected key ordering
- Repetition of keys
- Adding natural language alongside structured content
- Mixing data types

This folder documents how models perform under schema constraints.

---

## Methodology

Each prompt here includes:
- A defined schema (inline or as instruction)
- Edge cases (e.g. nested fields, optional keys, type enforcement)
- Evaluation of structure adherence
- Test logs per model/version

Models tested:
- GPT-4o, Claude 3 Opus, Grok-3  
- Validated manually or with simple parser (jq, Python `json.loads()`)

---

## Related work

This folder ties into:  
- `few-shot/` – few-shot examples that reinforce structure
- `live-projects/` – where these formats are used in deployed agents
