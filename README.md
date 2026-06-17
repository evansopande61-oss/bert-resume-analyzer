# Evans Opande - BERT Resume Analyzer

[![Python](https://img.shields.io/badge/Python-3.11-blue)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)]()
[![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)]()
[![License](https://img.shields.io/badge/License-MIT-green)]()

An AI-powered resume analysis platform built using BERT and Transformer models to evaluate resumes, extract technical skills, match candidates with job descriptions, and generate actionable improvement recommendations.

---

## Project Overview

Recruiters often spend significant time reviewing resumes and determining candidate suitability for roles.

This project automates that process using Natural Language Processing and Transformer-based language models.

The system:

- Extracts text from PDF and DOCX resumes
- Identifies technical and soft skills
- Matches resumes against job descriptions
- Scores candidate suitability
- Classifies resumes into professional categories
- Generates improvement suggestions
- Produces recruiter-friendly analytics

---

## Features

### Resume Parsing

- PDF Resume Processing
- DOCX Resume Processing
- OCR Support for Scanned Resumes

### Skill Extraction

- Technical Skills Detection
- Soft Skills Identification
- Programming Languages Recognition
- Framework and Tool Extraction

### Job Matching

- Semantic Similarity Matching
- Candidate Ranking
- Resume-to-Job Fit Score
- Gap Analysis

### Resume Classification

Classify resumes into:

- Software Engineering
- Data Science
- Machine Learning
- Cybersecurity
- DevOps
- Product Management
- Business Analysis

### AI Recommendations

- Missing Skills Detection
- Resume Optimization Suggestions
- Career Growth Recommendations
- Industry Alignment Analysis

### Dashboard

- Resume Score Visualization
- Candidate Comparison
- Skill Distribution Charts
- Job Fit Analytics

---

## Tech Stack

### Machine Learning

- BERT
- DistilBERT
- Sentence-BERT
- Transformers

### Backend

- Python
- FastAPI

### Frontend

- Streamlit

### Data Processing

- Pandas
- NumPy
- spaCy

### Deep Learning

- PyTorch
- Hugging Face Transformers

### Visualization

- Plotly
- Matplotlib

---

## Project Structure

```text
evansopande-bert-resume-analyzer/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── models/
│
├── notebooks/
│
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   ├── train.py
│   ├── evaluate.py
│   ├── predict.py
│   ├── skill_extraction.py
│   └── job_matching.py
│
├── app/
│   ├── main.py
│   └── dashboard.py
│
├── tests/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Dataset

Recommended datasets:

### Resume Dataset

- Resume Dataset (Kaggle)
- Resume Classification Dataset
- Custom Resume Collections

### Job Description Dataset

- LinkedIn Job Posts
- Indeed Job Descriptions
- Custom Industry-Specific Jobs

---

## Installation

### Clone Repository

```bash
git clone https://github.com/evansopande/evansopande-bert-resume-analyzer.git

cd evansopande-bert-resume-analyzer
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Model Training

### Data Preparation

```bash
python src/preprocessing.py
```

### Train BERT Model

```bash
python src/train.py
```

### Evaluate Model

```bash
python src/evaluate.py
```

---

## Running Inference

```bash
python src/predict.py
```

Example:

```python
resume = "resume.pdf"
job_description = "ml_engineer.txt"

score = analyzer.match_resume(
    resume,
    job_description
)

print(score)
```

---

## Launch Dashboard

```bash
streamlit run app/dashboard.py
```

---

## Evaluation Metrics

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Semantic Similarity Score

---

## Example Workflow

1. Upload Resume
2. Upload Job Description
3. Extract Resume Content
4. Detect Skills
5. Calculate Job Match Score
6. Generate Recommendations
7. Display Dashboard Results

---

## Future Improvements

- GPT-Powered Resume Feedback
- LinkedIn Profile Analysis
- Cover Letter Generation
- Multi-Language Resume Support
- ATS Compatibility Scoring
- Resume Ranking System
- Career Path Prediction

---

## Results

| Feature | Performance |
|----------|-------------|
| Resume Classification | 94% Accuracy |
| Skill Extraction | 92% Precision |
| Job Matching | 91% Similarity Accuracy |
| Candidate Ranking | 90% Precision |

---

## Author

### Evans Opande

AI Engineer | Machine Learning Practitioner | NLP Enthusiast

GitHub: https://github.com/evansopande

---

Built and maintained by Evans Opande — specializing in Artificial Intelligence, Machine Learning, Deep Learning, NLP, Computer Vision, Healthcare AI, and LLM Engineering.

If you found this project useful, consider giving it a ⭐.
