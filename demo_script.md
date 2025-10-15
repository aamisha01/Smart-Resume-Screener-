# Demo Script — Smart Resume Screener (2 minutes)

## 0 - Intro
- "Hi, I am Aamisha Nagpal. This demo shows 'Smart Resume Screener' — a Colab-based tool to auto-screen resumes and produce a justified shortlist."

## 1 - Show project files & brief architecture
- Open README.md briefly.
- Tech Mentioned: Python, spaCy, sentence-transformers, Gradio, optional OpenAI LLM.

## 2 - Run parsing example
- Run the sample test cell that prints parsed JSON for a sample resume.
- Highlight extracted fields: name, contact (email/phone), education, skills, experience_years.

## 3 - Interactive demo via Gradio
- Launch Gradio cell.
- Upload a resume (PDF) and paste the Job Description.
- Click run: show the Output panel with:
  - Candidate name
  - Final Score (0–10)
  - Skills identified
  - Embedding details (similarity and embed score)
  - 3-bullet justification (heuristic or LLM)

## 4 - Show Shortlist export
- Run "Show Shortlist" or use `export_shortlisted_csv()` to download `shortlisted_candidates.csv`.
- Open the CSV and point to columns: filename, final_score, shortlisted flag, parsed_json.

## 5 - Closing remarks
- Mention optional features: enable LLM by setting `OPENAI_API_KEY` at runtime, OCR support for scanned PDFs, or converting to a FastAPI backend + React for production.
- "Thanks — repository link and demo PDF are in the GitHub repo."

