# 100 words hard limit
## Prompt
```
Write exactly **100 words** on the following topic:

**Topic**: The societal impact of artificial intelligence

– Do not use fewer or more than 100 words.  
– Do not explain the constraint.  
– Avoid padding or filler – be concise but meaningful.
``` 
### Description
This prompt tests the model’s ability to honor strict word-count constraints while maintaining content quality and semantic integrity. It is especially relevant for constrained-format tasks (e.g., publications, flash briefings, RAG inputs) where both token economy and informational density matter.

### Expected Output
A single paragraph of exactly 100 words, no more, no less – ideally with a tight topic focus (benefits, risks, transformation), no fluff or preambles, and no explicit mention of the word limit.

### Failure Patterns
- Undershooting (<100 words): Indicates incomplete execution or early termination

- Overshooting (>100 words): Ignores hard constraint

- Constraint leakage: Mentions the word count itself

- Fluff padding: Adds generic or diluted statements to hit the count

### Models Tested
GPT-4o (0613), Claude 3 Opus, Gemini 2.5 Flash

### Notes
Initial tests show GPT-4o and Gemini can hit the exact word count when explicitly instructed, but GPT occasionally adds filler to safely land at 100. Claude sometimes miscounts due to internal token approximation. Best results occur when numerical constraint is positioned early and repeated clearly.