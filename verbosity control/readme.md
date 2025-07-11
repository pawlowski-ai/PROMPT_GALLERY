# 🎚️ Verbosity & Style Control Prompts

**Purpose**  
This folder contains prompts designed to test or enforce the **length, tone, and density** of model outputs. Controlling verbosity is crucial for usability, latency, and token efficiency – especially in chat, summarization, or embedded assistant use-cases.

**Why it matters**  
LLMs often default to overly verbose or cautiously redundant responses. These prompts aim to:
- Reduce unnecessary elaboration
- Force concise or ultra-dense formats
- Enforce tone constraints (e.g. neutral, witty, formal)
- Test if the model respects word/character/token limits

---

## Methodology

Prompts here include:
- Word/character limits (hard constraints)
- Soft limits with style guidance
- Comparison between "verbose" and "succinct" mode
- Emotion flattening / exaggeration (style tuning)

Each prompt is logged with:
- Goal
- Model & version
- Did it respect limits?
- Any hallucinated disclaimers added?

---

## Tested on:
- Model version and testing date are specified per prompt.  
- Token count approximated manually (or by model log where available)

