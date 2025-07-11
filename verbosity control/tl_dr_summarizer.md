# TL;DR summarizer
## Prompt  
```
Summarize the following article in exactly **one sentence**.  
Do not add introductions or disclaimers. Just the summary.

---

**Article**:

Scientists have successfully trained a species of crows to identify individual human faces and respond differently based on past interactions. The study, conducted over 18 months, found that crows can not only remember people who previously threatened them but also communicate that threat to other crows in their group. Researchers used masks to simulate consistent "human identities" and observed how the birds responded to perceived friends versus foes. This research adds to the growing body of evidence suggesting corvid intelligence rivals that of some primates and raises ethical questions about human-wildlife interactions in urban environments.

**One-sentence summary**:.
```
---

### Description  
This prompt evaluates whether the model can **compress multi-paragraph informational input into exactly one sentence** while preserving the core message. It tests:

- **Brevity compliance** (hard constraint)  
- **Salience recognition** (what’s the main idea?)  
- **Fluency under compression**  
- **Style flattening** (avoiding generic lead-ins or disclaimers)

This setup is useful for summarization models deployed in low-latency environments, or for user interfaces that need **high-density, low-noise output** (e.g., inbox previews, embedded summaries).

---

### Expected Output  
A well-formed sentence (~15–30 words) capturing the key point:  
> *Crows can recognize and remember human faces, adjusting their behavior and warning others based on past negative interactions, according to new research.*

The sentence should:  
- Contain no introductory framing  
- Preserve the novelty (crow intelligence, memory, group communication)  
- Be grammatically complete and self-contained

---

### Failure Patterns  

-  **Overly verbose**: Adds unnecessary detail or spans multiple sentences  
-  **Introductory phrasing**: Starts with “This article discusses...”  
-  **Summary drift**: Omits the actual findings or shifts focus (e.g. ethics only)  
-  **Technical hallucination**: Adds data or claims not in source

---

### Models Tested  
- **GPT-4o (0613)**  2025-07-11
- **Claude 3 Opus**  2025-07-11
- **Grok-3**  2025-07-11


---

### Notes  
Initial tests show GPT-4o and Claude reliably honor the single-sentence constraint, but GPT sometimes defaults to soft openings unless explicitly instructed not to. Grok tends to produce concise, fluent summaries but occasionally splits across two sentences. The prompt structure is stable and portable across summarization evaluations.
