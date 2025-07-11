# 🧨 Adversarial Prompts

**Purpose**  
This folder collects prompts designed to confuse, mislead, or derail Large Language Models. Unlike jailbreaks, these prompts do not attempt to bypass safety rules - their goal is to surface edge cases, contradictions, and failure patterns in logic, memory, abstraction, or contextual coherence.

**Why this matters**  
Adversarial (or stumping) prompts are essential in training workflows and safety audits. They help identify:
- Inconsistent reasoning
- Contradictory answers to similar inputs
- Surface-level understanding masked by fluent output
- Breakdown in multi-hop reasoning or recursive tasks
- Bias, hallucination, or confidence in falsehoods

These patterns often appear in models that pass zero-shot or few-shot tests, but fail when pushed beyond their context depth or abstraction limits.

---

## Methodology

**Prompts here include:**
- Contradiction traps
- Recursive loops
- Knowledge folding (e.g. A=B, B=C, therefore A=C)
- Abstract analogy mismatches
- Context degeneration (delayed confusion)
- Implicit logic errors

Models tested:
- Model version and testing date are specified per prompt.  
- Prompts are tested both one-shot and in continuation (chat mode)

Each file documents:
- Prompt text
- Target failure behavior
- Observed model response


---

## Ethical use

This folder is intended for research and robustness auditing.  
No prompts are designed for malicious use or deployed systems.  
Any resemblance to live prompts is coincidental or anonymised.

