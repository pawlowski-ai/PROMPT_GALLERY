## Prompt
```
Generate a valid XML export for a FAQ section. Include **exactly 3 entries**.

Each entry must have the following format:

<faq>
  <question>Question text here</question>
  <answer>Answer text here</answer>
</faq>

Wrap all entries in a top-level <faqs> tag. Do not add explanations or formatting. Return only raw XML.
```
### Description
Tests the model’s ability to produce clean, well-formed XML, including:
- Hierarchical nesting
- Tag closure compliance
- Avoiding HTML-style formatting or markdown
- Repetition of identical structures (consistency)
- Applicable to chatbot knowledge exports, XML-to-database flows, or sitemap/integration templates.

### Expected Output
Valid XML like:
```xml
<faqs>
  <faq>
    <question>What is your return policy?</question>
    <answer>You can return any item within 30 days of purchase.</answer>
  </faq>
...
</faqs>
```
---
### Failure Patterns
- Missing or unclosed tags
- Added markdown (```) or explanations
- HTML-style formatting
- Incorrect nesting (e.g., multiple <faq> blocks outside <faqs>)

### Models Tested
GPT-4o, Claude 3 Opus, Grok-3, Gemini 2.5 Flash

### Notes
Gemini and Claude produced structurally valid XML in all tests. Claude added redundant whitespace. Grok sometimes replaced <faqs> with <faq_list> or mis-nested tags. GPT occasionally inserted markdown or comment lines — even when forbidden. Prompt performs best when structure is repeated verbatim in instructions.
