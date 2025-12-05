# Change Log
- Added summary_level variable with conditional logic for "short" and "detailed" summaries.
  
Module 2: Section Loop
For each section:
Summarize in ≤50 words.
Use bullet points.
Track cumulative word count (≤200 words).

## Section Loop Logic
- Introduce variable: `summary_level` (values: "short" or "detailed").
- For each section:
  - If `summary_level = "short"`:
    - Generate a compact 1–2 sentence summary.
  - If `summary_level = "detailed"`:
    - Generate a short paragraph summary.
    - Add a bullet list of 3–5 key points highlighting important details.
- Ensure word count constraints are respected.





