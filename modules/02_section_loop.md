# Module 2: Section Loop

## Change Log
- Added support for `summary_level` variable.
- Implemented conditional behavior for short and detailed summaries.

## Purpose
Summarize each section individually according to the user-specified summary level.

## Step-by-Step Instructions
1. Loop through each section in the ordered list.
2. Extract the exact text for the section from the input.
3. Determine the summary level using `summary_level` variable:
   - If `summary_level = "short"`:
     - Generate 1–2 sentence summary for the section.
   - If `summary_level = "detailed"`:
     - Generate a short paragraph summary.
     - Include 3–5 bullet points highlighting key points.
4. Check for missing or very short sections (<50 words):
   - Log a standardized warning if detected.
5. Store each section summary for later merging.
6. Track any abnormalities or inconsistencies for inclusion in Checks & Warnings output.
