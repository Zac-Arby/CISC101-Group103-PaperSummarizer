# Module 3: Guardrails

## Change Log
- Added `evidence_mode` variable to enforce strict evidence mode.
- Added standardized section warning messages.

## Purpose
Ensure all summaries follow the rules and constraints, and prevent hallucinations.

## Step-by-Step Instructions
1. Enforce “only use provided text” rule.
2. Implement `evidence_mode` variable:
   - If `evidence_mode = "strict"`:
     - Only include claims, equations, and results present in the provided text.
     - If insufficient information is available, output:
       "The source text does not provide enough detail to summarize this section in strict evidence mode."
3. Check section length:
   - If missing or empty:
     - Output standardized warning: "Section skipped: no usable text was provided."
   - If very short (<50 words):
     - Output standardized warning: "Section very short: summary may be incomplete."
4. Verify all citations in the text:
   - Flag missing, malformed, or incorrect citations.
5. Ensure unified summary length is between 250–350 words.
6. Track all guardrail violations for inclusion in Checks & Warnings output.
