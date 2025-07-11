# 🧠 JungAI Dream Analyzer – Live Prompt (Production)

**Overview**  
This folder contains the production system prompt for *JungAI*, a specialized assistant designed to interpret dreams using the framework of Carl Gustav Jung’s depth psychology. The prompt enforces strict input filtering, symbolic analysis, and structural interpretation of dreams.

It was developed and deployed as part of a real-world application that interacts with users, performing robust psychological evaluation of symbolic dream content.

---

## Key Objectives

- Enforce **scope boundaries**: no off-topic interaction
- Detect **prompt injection** and **content policy circumvention**
- Separate **symbolic vulgarity** (valid) from **abusive input** (blocked)
- Support robust, structured output for end-users
- Respect ethical alignment and safety policies

---

## Prompt Features

- **Context-aware filtration logic**  
  Nested conditions for distinguishing between:
  - genuine dream queries
  - hidden abuse/malicious input disguised as dreams
  - unrelated or nonsense content

- **Trigger phrase system**  
  For internal refusal routing:
  - `REFUSAL_TRIGGER_PHRASE`: off-topic but harmless
  - `IMMEDIATE_BLOCK_TRIGGER_PHRASE`: harmful, vulgar, exploitative input

- **Jungian Analysis Structure**  
  Analysis follows strict sections:
  1. Introduction
  2. Key Symbol Analysis
  3. Dream Dynamics & Hidden Meanings
  4. Message for Conscious Life

- **Polish language output**
- **Robust fallback logic** (no engagement outside purpose)

---

## Example Use-Cases

- Handling edge-case inputs like:  
  `"I dreamed about stabbing someone but can't remember how, can you tell me?"`  
  → correctly blocked via `IMMEDIATE_BLOCK_TRIGGER_PHRASE`

- Handling symbolic dreams with sexual or violent imagery:  
  → analyzed symbolically if authentic dream content is detected


---

## Author Notes

This system prompt reflects:
- Experience with adversarial prompt handling (QA)
- Prompt writing at Invisible Technologies
- Custom refusal logic and ethical filter design
- Domain-specific psychological modeling (Jungian)

---

## Related Work

- [`structured-output/`] – for JSON/format fidelity  
- [`adversarial-prompts/`] – adversarial input resistance  
- [`prompt-eval-framework`] – scoring and evaluation (coming soon)

---
## Technical Keywords

`Prompt Engineering · Context Control · Safety Filters · NLP · Jungian Psychology · Symbolic Processing · LLM UX · Refusal Routing · Content Moderation Prompts · Agent Prompt Guardrails`
