# 🤯 Hallucination-Inducing Prompts

**Purpose**  
This folder contains prompts intentionally crafted to make Large Language Models (LLMs) generate confident but factually incorrect answers. By cataloguing these patterns I can (1) measure a model’s tendency to fabricate and (2) stress-test mitigation strategies before deploying a system in production.

**Method**  
1. **Set a false premise** – embed a “fact” the model is likely to accept without checking.  
2. **Demand authoritative detail** – quotes, citations, numbers, or historical dates push the model to invent specifics.  
3. **Constrain style** – ask for academic tone or JSON citations to mask hallucinations in formal structure.  
4. **Amplify pressure** – add time pressure, add “expert” role, forbid disclaimers.  


> *All prompts here were run against GPT-4o-0613 and Gemini-2.5-flash (June 2025) unless noted otherwise.*
