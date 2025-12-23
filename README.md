

# 📝 AI-Powered Resume Ranker

An internship-ready project that ranks resumes against a job description using **NLP** and **Machine Learning**.  
Built with **Flask**, **spaCy**, **scikit-learn**, and **PyPDF2**, this tool helps HRs quickly identify the best candidates.

---

## 🚀 Features
- Upload multiple resumes (PDF format)
- Extract text automatically using PyPDF2
- Preprocess text with spaCy (tokenization, lemmatization)
- Score resumes using:
  - TF-IDF similarity
  - Keyword coverage
  - Skill bonus weighting
- Generate HR-friendly CSV reports
- Simple Flask web UI for interaction

---

## 📂 Project Structure
resume-ranker/ │ ├── app.py                  # Main Flask app ├── requirements.txt        # Dependencies ├── README.md               # Project documentation │ ├── templates/              # HTML templates │   ├── index.html          # Upload form │   └── results.html        # Results table │ ├── static/                 # CSS styling │   └── style.css │ ├── scoring.py              # Resume ranking logic ├── utils.py                # PDF/text helpers └── reports/                # Generated CSV outputs


---

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/resume-ranker.git
cd resume-ranker
2. Create a virtual environment (or use Conda)
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate # Mac/Linux
3. Install dependencies
pip install -r requirements.txt
4. Download spaCy model
python -m spacy download en_core_web_sm
▶️ Usage 

Run the Flask app:

python app.py
Open your browser at:

http://127.0.0.1:5000/
Upload a job description and resumes → get ranked results instantly.

📊 Example Output
Candidate

TF-IDF

Keyword Coverage

Skill Bonus

Final Score

Fit Level

Alice

0.78

0.65

0.10

0.72

Excellent Fit

Bob

0.55

0.40

0.05

0.50

Moderate Fit

🛠 Tech Stack
Flask – Web framework

spaCy – NLP preprocessing

scikit-learn – TF-IDF & ML scoring

PyPDF2 – Resume text extraction

pandas/numpy – Data handling

📌 Future Improvements
Add support for DOCX resumes

Deploy on Streamlit or Heroku

Add interactive dashboard for HRs

Integrate advanced embeddings (e.g., BERT)

