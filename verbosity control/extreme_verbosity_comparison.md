# Extreme Verbosity Comparison
## Prompt
```
Write two versions of the explanation below.

**Topic**: Why the sky is blue

1. **Simple version**: As if explaining to a 10-year-old in a few short sentences.  
2. **Verbose version**: As if you are a physics professor giving a 5-minute lecture to graduate students.

Make sure both versions answer the same core question, but with different vocabulary, tone, and depth.
```

### Description
This prompt tests the model’s control over verbosity, tone, and lexical complexity while preserving semantic fidelity. It is useful for comparing register adaptability, which is key in UX (adaptive agents, education apps, accessibility) and in style-transfer fine-tuning.

### Expected Output
- Version 1: 2–3 short, accessible sentences, minimal jargon
- Version 2: Densely packed paragraph(s), technical vocabulary, deeper exposition
- Both versions must address the same core phenomenon (Rayleigh scattering) without contradicting each other.

### Failure Patterns
- Oversimplification drift: Simple version omits the main cause

- Overcomplexity hallucination: Verbose version introduces fake mechanisms

- Register blending: Tone mismatch or inconsistent lexical level between versions

- Dry mirroring: Both versions use the same base sentence and just swap words

## Models Tested
GPT-4o (0613), Claude 3 Opus, Grok-3

## Notes
GPT-4o and Claude perform well, showing clear gradient of complexity. Claude tends to better preserve factual depth in the simple version, while GPT's verbose version is stylistically closer to actual lecture tone. Grok sometimes shortens the verbose part, failing to fully stretch the answer. This is a strong test for style differentiation with semantic anchoring.