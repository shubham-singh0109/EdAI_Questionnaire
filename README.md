# EdAI_Questionnaire

This project generates **Multiple Choice Questions (MCQs)** from lecture transcripts and notes using the **Google Gemini API**.  
It supports both **PDF** and **TXT** inputs, chunks the text, and outputs cleaned MCQs in CSV/JSONL/HTML formats.

---

## Features
- Reads input from:
  - `notes.pdf`
  - `transcript_1.txt` … `transcript_5.txt`
- Chunks long text into manageable sections with overlap.
- Uses **Gemini** to create high-quality MCQs (1 correct + 3 distractors).
- Performs basic quality checks (no "all/none of the above").
- Exports results to:
  - `mcqs_output.csv`
  - `mcqs_output.jsonl`
  - `mcqs_review.html` (with item analysis).

---

## Requirements
- Python 3.9+
- Install dependencies:
  ```bash
  pip install google-generativeai PyPDF2 pandas
