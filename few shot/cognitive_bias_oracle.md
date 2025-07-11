# Prompt  
```
Confirmation bias = Mirror  
Anchoring bias = Boulder  
Dunning-Kruger effect = Megaphone  
Framing effect = Window  
Sunk cost fallacy = Trapdoor  
Fundamental attribution error = Spotlight  

---
[Your Turn]
Self-serving bias =  
Negativity bias =  
Bandwagon effect =  
Halo effect =  
Choice-supportive bias =  
```
---

### Description  
This few-shot prompt presents a structured mapping between **cognitive biases and symbolic metaphors**, using single-word or conceptual labels. It provides no instructions or role definitions, requiring the model to **infer the mapping logic purely from examples**. The goal is to test the model's ability to perform **conceptual analogy abstraction**: mapping psychological mechanisms to metaphorical objects that capture their underlying logic or function.

This setup is valuable for:  
– evaluating interpretative reasoning  
– testing analogical metaphor generation  
– constructing creative educational datasets on cognitive biases

---

### Models Tested  
- **ChatGPT-4o (0613)** – tested 2025-07-11  
- **Gemini 2.5 Pro** – tested 2025-07-11

---

### Notes  
- **GPT-4o** provided a conversational-style completion, beginning with a natural language preamble and then mapping each bias to a metaphor. Each mapping included a **brief rationale**, explaining the symbolic logic behind the assigned word.  
  - Example: `Bandwagon effect = Wave ("A wave sweeps people up and carries them along — just like the bandwagon effect pulls individuals to adopt beliefs or behaviors because many others are doing so.")`  
  - Demonstrated high interpretability, but slightly broke the minimalist pattern.

- **Gemini 2.5 Pro** adhered strictly to the established format (`bias = word`) without any commentary or preamble.  
  - Mappings were **structurally consistent and conceptually accurate**, indicating that the model correctly inferred the abstract mapping logic from the few-shot examples.  
  - Strong adherence to form shows Gemini’s strength in **format compliance and latent pattern recognition**, even without explicit instruction.

- Both models **successfully adapted to the prompt’s implicit logic**, indicating robust abstraction abilities.  
- The prompt is a reliable scaffold for testing **conceptual compression and analogical reasoning** without direct supervision.

