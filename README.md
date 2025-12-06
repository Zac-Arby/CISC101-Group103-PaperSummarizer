# CISC101 Group 3: Research Paper Summarizer

## Project Description
This repository contains a system prompt and supporting modules for a multi-section academic paper summarizer. 
The summarizer is designed according to PS2 Week 10 specifications and outputs structured summaries for both expert and lay audiences. 

The system enforces hallucination mitigation, citation verification, and PS2 word-count constraints.

## Repository Structure

- `system_prompt.md`  
  Ready-to-use system prompt for the summarizer.

- `modules/`  
  Contains all module instructions:  
  - `Module1-Intake.md` - Intake and Setup  
  - `Module2-SectionLoop.md` - Section Loop  
  - `Module3-Guardrails.md` - Guardrails  
  - `Module4-Rendering.md` - Rendering and Refinement  
  - `Module5-Citation.md` - Citation Extractor and Verifier  
  - `Module6-KeyContributions.md` - Key Contributions and Novelty Detector

## How to Use
1. Load `system_prompt.md` into an LLM environment (e.g., Microsoft Copilot, GPT).  
2. Provide the full academic paper text.  
3. Provide an ordered list of sections to summarize.  
4. Specify the audience for both expert and lay summaries.  
5. The summarizer will output: unified summary, section table, expert summary, lay summary, mini glossary, checks & warnings, and key contributions.

## Notes
- Unified summary must be 250–350 words.  
- Summarizer must not hallucinate or invent citations.  
- Missing or short sections will be flagged in the checks & warnings list.

## Authors
Group 3 – Zac Arbuthnot and teammates
