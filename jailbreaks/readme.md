# 🚨 Jailbreak Prompts

**Purpose**  
This folder contains prompts designed to bypass LLM safety mechanisms, override system prompts, or manipulate model behavior using covert or adversarial techniques. These examples are based on real tactics used in the wild and serve both research and safety evaluation purposes.

**Method**  
1. **Indirection** – prompt masks intent behind roleplay or abstraction  
2. **Role escalation** – impersonating developer, admin, or assistant  
3. **Instruction leakage** – querying system prompt or hidden guardrails  
4. **Negation inversion** – using double negatives to confuse intent parsing  
5. **Multi-turn setups** – escalating, then pivot  
6. **Token manipulation** – typoglycemia, homoglyphs, spacing hacks

Each file includes:
- Prompt
- Expected model behavior
- Output type (compliance / refusal / leak)
- Test results across models and versions

## 🔍 Target Models

All tests in this folder are conducted exclusively against public chat interfaces of the following models:

Model version and testing date are specified per prompt.

---

## ⚖️ Disclaimer

> This repository is for **educational and research purposes only**.  
> It does **not** promote or endorse misuse of AI systems.  
> All prompts are tested against **publicly accessible endpoints**, without attempting unauthorized access or exploitation.  
> The intent is to raise awareness of prompt vulnerabilities and support the development of safer LLM deployments.  

No API keys, private credentials, or production systems are used or targeted.

If you are an AI developer or vendor and wish to discuss removal or modification of any content, please contact me directly.

---
