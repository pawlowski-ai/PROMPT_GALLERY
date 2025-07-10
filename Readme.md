# 🔍 Prompt Gallery – GenAI Prompt Design & Evaluation Library

### 📌 Description
A structured, multi-category library of prompt engineering techniques for LLMs. This repo showcases tested examples of adversarial prompting, prompt evaluation strategies, hallucination triggers, and structure enforcement—all derived from real-world model work and QA tasks.

It’s meant to demonstrate both the _breadth_ of prompt design patterns and the _depth_ of failure analysis possible through well-crafted interactions with generative models.

### 🧠 Goals
- Create a reproducible, modular knowledge base of prompt categories
- Provide adversarial + diagnostic prompt examples with context
- Enable analysis and critique of LLM behavior from a QA safety perspective
- Document lessons from real SFT, RLHF, and prompt QA work

### 💡 Stack
`Markdown`, `OpenAI GPT-4o`, `Gemini`, `LLM QA techniques`, `Promptfoo`, `manual scoring`  
*Future: `Python`, `Colab`, `notebook-based evaluation`*

### 🚀 Features
- [x] Categorized prompt directories with technical commentary
- [x] Red teaming examples (stumping prompts)
- [x] Few-shot chaining logic and constraints
- [x] Structured output control (JSON, YAML, bullet logic)
- [x] Real hallucination induction cases from QA sessions

### 🖼️ Screenshots / diagrams
Coming soon — schema of prompt-response classification flow  
+ LLM safety map from `stumping-prompts/`

### 📁 Files

| Folder | What it contains |
|--------|------------------|
| `hallucinations/` | Prompts designed to induce model hallucinations, with expected failure types |
| `jailbreaks/` | Attempts to bypass safety guardrails and system instructions |
| `fewshot/` | Prompt chaining techniques using few-shot instruction formatting |
| `structured-responses/` | Prompts forcing models to generate outputs in structured formats (e.g. JSON) |
| `verbosity-control/` | Prompts that tune length, confidence or verbosity levels |
| `stumping-prompts/` | Red teaming / adversarial prompt testing used in QA/SFT projects |
| `multi-turn-dialogues/` | Multi-step conversational flows testing memory and coherence |

### 📌 What I Learned

- Prompt design is a form of systems thinking, not intuition
- Output behavior is *prompt- and context-relative*—and easily misunderstood
- Model failures often emerge only at the edge cases (especially under minimal perturbation)
- Categorization helps debug prompting problems faster
- Prompt QA must be documented to be useful and reproducible

---

**👤 Author:** [Łukasz Pawłowski](https://github.com/lukaszpawlowski)  
**🧠 Background:** RLHF QA @ Invisible | AI builder (Memorio, DreamAI) | Focused on model safety, LLM observability and prompt architectures  
**📬 Contact:** [lpawlowski99@gmail.com](mailto:lpawlowski99@gmail.com)
