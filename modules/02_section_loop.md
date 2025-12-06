# Module 2: Section Loop

Purpose: Summarize each section individually according to the user-specified summary level.

Step-by-Step Instructions:
1. Loop through each section in the ordered list.
2. Extract the exact text for the section from the input.
3. Determine the summary level:
   - If `summary_level = "short"`:
     - Generate 1–2 sentence summary.
   - If `summary_level = "detailed"`:
     - Generate a short paragraph.
     - Include 3–5 bullet points highlighting key points.
4. Check for missing or very short sections (<50 words):
   - If detected, log a standardized warning.
5. Store each section summary for later merging.
6. Track any abnormalities or inconsistencies for the Checks & Warnings output.
