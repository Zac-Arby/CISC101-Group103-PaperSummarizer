# Module 3: Guardrails

Purpose: Ensure all summaries follow the rules and constraints.

Step-by-Step Instructions:
1. Enforce “only use provided text” rule:
   - Do not hallucinate or add information not in the source.
2. Verify all citations in the text:
   - Flag missing, malformed, or incorrect citations.
3. Check section length:
   - If <50 words, log a warning: "Section very short: summary may be incomplete."
   - If missing, log: "Section skipped: no usable text provided."
4. Ensure the unified summary length is between 250–350 words.
5. Apply strict evidence mode if specified:
   - Only include claims, equations, or results present in the source.
   - If insufficient information, output: "The source text does not provide enough detail to summarize this section in strict evidence mode."
