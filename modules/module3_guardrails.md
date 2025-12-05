Module 3: Guardrails
Flag missing or empty sections.

Flag sections <50 words.
## Guardrails
- Introduce variable: `evidence_mode` (values: "strict" or "default").
- If `evidence_mode = "strict"`:
  - Summarizer must only include claims, equations, and results explicitly present in the source text.
  - If insufficient information is found:
    - Output: “The source text does not provide enough detail to summarize this section in strict evidence mode.”
- Section Warnings:
  - If section is missing or empty:
    - Output: “Section skipped: no usable text was found.”
  - If section < 50 words:
    - Output: “Section too short: summary may be incomplete.”

Apply hallucination mitigation (summarize only present content).

Apply long-paper chunking if input exceeds context window.
