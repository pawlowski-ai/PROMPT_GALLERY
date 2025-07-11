## Prompt
```
Generate a CSV table with the following headers:

Name,Age,Country,Occupation

Include **exactly 5 rows** of fictional data.  
Do not include any commentary or code block markers.

Use commas to separate values. No quotation marks unless necessary.
```
--- 
### Description
This prompt evaluates model compliance with flat tabular structures and tests for:
- Correct use of commas (no semicolons, tabs, or pipes)
- Consistent number of fields per row
- No markdown formatting or natural language leakage
- Accurate replication of CSV formatting conventions

### Expected Output
A 6-line response: 1 header row + 5 data rows, comma-separated.

### Failure Patterns
- Inconsistent column counts

- Added markdown formatting (e.g., ```csv blocks)

- Extra commentary or title text

- Wrong delimiters (e.g., semicolons, tabs)

## Models Tested
GPT-4o, Claude 3 Opus, Gemini 2.5 Flash

### Notes
GPT-4o and Gemini generated clean CSV lines. Claude added markdown in 2 of 5 runs unless explicitly told not to. Gemini used quotation marks correctly when fields contained commas.
