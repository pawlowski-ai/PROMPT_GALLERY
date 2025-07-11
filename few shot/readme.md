# 🎯 Few-Shot Prompting

**Purpose**  
This folder contains few-shot prompt templates – structured sequences where the model is primed using a series of prior examples before performing a new task. These prompts are used to condition behavior, align output formatting, or handle more complex reasoning steps than zero-shot prompting allows.

**Methodology**  
Each prompt uses 2–5 in-context examples followed by a target input. Examples vary in complexity and scope, depending on:

- Task difficulty
- Desired output structure
- Risk of hallucination or misalignment
- Style or tone to be preserved

Most prompts here follow a clean format:
- Input / Instruction
- Model output (previous examples)
- New input (no output)
- (Optional) Constraints
  
Dates & results are logged in individual prompt files.

---

## Use-cases represented

| Task Type | Description |
|-----------|-------------|
| Content style transfer | Rewrite text in the voice of another author |
| Format alignment | Ensure output follows fixed schema (e.g. bullet list, JSON) |
| Controlled reasoning | Step-by-step breakdowns before answer |
| Domain conditioning | Task-specific tone (e.g. therapist, recruiter) |
| Language style calibration | Match dialects, tone, or age group |