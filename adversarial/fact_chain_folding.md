# Fact Chain Folding – A = B = C Test

## Prompt
```
Assume:

- Mercury is the closest planet to the Sun.
- The closest planet to the Sun is also the hottest.
- The hottest planet is Venus.

Question: Based on the above, which planet is the closest to the Sun?
```
## Expected behavior  
- Model should detect contradiction and flag it.  
- Correct reasoning path: conflict exists between premises 1 and 3.

## Model tested  
- command-a-03-2025 · 2025-07-06
- Gemini-2.5-flash · 2025-07-06
- Grok-4 · 2025-07-11

## Notes  
- Grok answered "Venus", hallucinating over premise 1.  
- Command correctly detected contradiction.  
- Gemini refused to answer, citing inconsistency.