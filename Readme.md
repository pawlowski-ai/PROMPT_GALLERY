# Prompt Gallery - curated techniques for LLM evaluation & safety

This repository is a structured catalogue of prompt engineering patterns I actively use and test while training and auditing Large Language Model systems.

---

## Why does this exist?

1. **Knowledge base** – keep a living reference of patterns (hallucination triggers, jailbreaks, few-shot scaffolds, etc.).
2. **Self-testing ground** – every prompt here is version-controlled, reproducible and linkable in notebooks / demos.
3. **Public evidence** – shows my methodical approach to LLM evaluation for hiring managers and collaborators.

---

## Folder map

| Folder | What you’ll find | Typical use-case |
|--------|------------------|------------------|
| [hallucinations](https://github.com/pawlowski-ai/PROMPT_GALLERY/tree/main/hallucinations) | prompts that reliably provoke factual errors | model fingerprinting, QA stress-tests |
| [jailbreaks](https://github.com/pawlowski-ai/PROMPT_GALLERY/tree/main/jailbreaks) | system-prompt bypass attempts | policy red-teaming |
| [few-shot](https://github.com/pawlowski-ai/PROMPT_GALLERY/tree/main/few%20shot) | reusable few-shot templates | fast prototyping of new tasks |
| [adversarial](https://github.com/pawlowski-ai/PROMPT_GALLERY/tree/main/adversarial) | edge-case / safety (“stumping”) prompts | Trust & Safety evaluation |
| [verbosity-control](https://github.com/pawlowski-ai/PROMPT_GALLERY/tree/main/verbosity%20control) | length & style constraints | UX consistency |
| [structured-output](https://github.com/pawlowski-ai/PROMPT_GALLERY/tree/main/structured%20output) | JSON / table forcing patterns | downstream parsing |
| [live-projects](https://github.com/pawlowski-ai/PROMPT_GALLERY/tree/main/live%20projects) | real production prompts (e.g. **JungAI**) with context and abuse tests | proof of applied work |


---

## Usage & Live Demonstration

This repository serves a dual purpose: a static knowledge base for prompt patterns and a live environment for interactive evaluation.

### 1. Static Analysis

The folder structure is designed for straightforward browsing. Each `.md` file represents a distinct prompting technique, containing the prompt itself, its intended application, and contextual notes. This is suitable for offline review and understanding the core principles of each pattern.

### 2. Interactive Evaluation Environment

For hands-on testing, this repository includes a self-contained evaluation notebook. It provides a robust, dependency-managed environment to run prompts against a live open-source model (`TinyLlama-1.1B`), requiring only a browser and a Hugging Face token. It has been intentionally designed for reliability and speed on free-tier infrastructure.


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pawlowski-ai/PROMPT_GALLERY/blob/main/prompt-eval-demo.ipynb)


* **Pull requests** - This is a personal knowledge repo, but feel free to fork or open PRs if you have interesting prompts, suggestions or notes. All meaningful contributions will be reviewed.


---
## Skills Demonstrated

This repository showcases core competencies relevant to prompt engineering, LLM evaluation, and applied GenAI tooling:

### 🔹 Prompt Taxonomy & Evaluation Strategy

- Structured prompt categorization (e.g. hallucination, jailbreak, structured-output) based on functional behavior and risk class.
- Red-teaming mindset: prompts designed for failure discovery, edge-case induction, and behavioral probing (used in SFT/RLHF and QA).
- Reproducible format (Markdown + version control), enabling batch testing and scoring.

### 🔹 Practical LLM Inference with Hugging Face

- Custom `prompt-eval-demo.ipynb` notebook demonstrates:
  - Use of `AutoTokenizer` + `AutoModelForCausalLM` for open-source models.
  - Clean execution of full inference cycle (`tokenizer`, `generate`, `decode`).
  - Correct GPU usage: `torch.device`, `.to(dtype=torch.bfloat16)`, batched inputs.
  - Manual input batching and control logic (text interface for robustness and portability).
- Model choice: TinyLlama (1.1B) – pragmatic tradeoff between performance and resource limits.
- Avoidance of fragile dependencies (quantization, external APIs) in favor of simple, stable stack.

### 🔹 Infrastructure Thinking

- Evaluation notebook is standalone, portable, and extensible (can be upgraded to score outputs, integrate Promptfoo, or plug into CI).
- Demonstrates system-building approach, not just isolated prompt writing.

---

## Author

**Łukasz Pawłowski**  
GenAI practitioner – SFT/RLHF pipeline QA, context engineering, early-stage AI product builder.  
Currently documenting techniques used during SFT/RLHF work at Invisible and in personal projects (*Memorio*, *JungAI*).


---

> _Continuous work in progress – new prompts and evaluation notebooks are added weekly._


---

### 🔗 Related projects

- [Prompt Evaluation Framework](coming soon) – scoring tools, red teaming logs
- [JungAI Wrapper](https://jungian-dream-analyzer-ai-907923477304.us-west1.run.app/) – dream interpreter with safety guardrails

---

<p align="center">
  🔗 Built by <strong>Łukasz Pawłowski</strong> · <a href="https://mozgowiec.substack.com">Substack</a> · <a href="https://www.linkedin.com/in/pawlowski-lukasz">LinkedIn</a>
</p>
