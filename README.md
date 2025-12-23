# Elevate_resume-ranker
# AI-Powered Resume Ranker

This project ranks resumes against a job description using NLP and ML techniques.

## 🚀 Features
- Upload multiple resumes (PDF)
- Extract text using PyPDF2
- Preprocess with spaCy
- Score resumes using TF-IDF + keyword coverage
- Generate HR-friendly CSV reports
- Flask web UI for easy use

## 📂 Project Structure
- `app.py` → Flask server
- `templates/` → HTML frontend
- `static/` → CSS styling
- `scoring.py` → Resume ranking logic
- `utils.py` → PDF/text helpers
- `reports/` → Generated CSV outputs

## ⚙️ Setup
```bash
conda create -n resume-ranker python=3.10
conda activate resume-ranker
pip install -r requirements.txt
python -m spacy download en_core_web_sm
