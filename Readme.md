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

## How to use this repo

* Browse folders → open any prompt file (`*.md` or `*.txt`) to view the instruction, expected behaviour and notes.  
* Run `notebooks/prompt-eval-demo.ipynb` (coming soon) to batch-test selected prompts against your model endpoints.
* File naming convention: `p{NN}_{slug}.md` for easy referencing.
* **Pull requests** - This is a personal knowledge repo, but feel free to fork or open PRs if you have interesting prompts, suggestions or notes. All meaningful contributions will be reviewed.


---

## Skills / methods demonstrated here

* Prompt taxonomy design (hallucination, jailbreak, structured, etc.)
* Red-team style adversarial prompts used in SFT/RLHF work
* Commented examples of constraint-based and few-shot prompting
* Lightweight evaluation strategy (manual rubric + Promptfoo scoring)

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
