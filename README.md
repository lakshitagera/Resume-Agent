# 🤖 Resume Agent – Your AI-Powered Job Application Assistant  

Resume Agent is an AI-powered application designed to improve resumes, discover relevant job opportunities, and generate personalized cover letters using NLP and modern Large Language Models (LLMs).  
This project aims to simplify the job application journey and help job seekers increase their chances of getting shortlisted.  

---

## 📸 Project Preview  
*(Add your actual screenshots in the below section — these placeholders indicate where they go.)*

![Resume Agent Banner](https://via.placeholder.com/1000x350.png?text=Resume+Agent)

---

## 📖 Overview  

In today’s competitive job market, over **75% of resumes are filtered out by Applicant Tracking Systems (ATS)** before a recruiter even views them.  
Resume Agent solves this by providing:

- **Resume improvement using NLP**  
- **Tailored job discovery using APIs**  
- **AI-generated professional cover letters**  

The system integrates Streamlit, Flask, Gemini AI, and JSearch API to deliver an end-to-end job-application assistant.  
(Information summarized from project report :contentReference[oaicite:1]{index=1})

---

## 🎯 Features  

### ✅ 1. Resume Improvement  
- Upload PDF/DOCX  
- AI analyzes structure, clarity, keyword relevance  
- Suggestions to improve ATS score  
- Highlights missing achievements, skills, quantifiable results  
(Ref: Resume improvement module description, page 11–15 :contentReference[oaicite:2]{index=2})

---

### ✅ 2. Job Discovery  
- Enter domain & location  
- System fetches real-time job listings using **JSearch API**  
- Shows job title, company, location, job description & apply link  
(Ref: Job discovery section, page 16–18 :contentReference[oaicite:3]{index=3})

---

### ✅ 3. Cover Letter Generation  
- Enter job role & company  
- AI creates a polished, role-specific formal cover letter  
- Ready for use or further editing  
(Ref: Cover letter module, page 19–20 :contentReference[oaicite:4]{index=4})

---

## 🏗️ System Architecture  
According to the workflow diagram on page 8 :contentReference[oaicite:5]{index=5}:

1. User uploads resume  
2. System extracts text (pdfplumber)  
3. User selects action  
4. Backend interacts with LLM / API  
5. Output displayed via Streamlit  

---

## 🧩 Modules  

| Module | Description |
|--------|-------------|
| **Resume Parser** | Extracts text from PDF/DOCX using pdfplumber |
| **Resume Improver** | Uses Gemini Flash LLM to analyze & suggest improvements |
| **Job Discovery** | Uses RapidAPI JSearch API |
| **Cover Letter Generator** | AI-writes customized cover letters |
| **Frontend** | Streamlit |
| **Backend** | Flask REST API |

(All modules taken from pages 8–12 of the PDF :contentReference[oaicite:6]{index=6})

---

## 🛠️ Technology Stack  

| Component | Tools Used |
|----------|------------|
| Frontend | Streamlit |
| Backend | Flask |
| Resume Parsing | pdfplumber |
| AI Models | Gemini Flash, Agno Agents |
| Job Search | JSearch API (RapidAPI) |
| Integration | REST APIs |

(Ref: Tech stack, page 21 :contentReference[oaicite:7]{index=7})

---

## 🚀 Installation & Setup  
1. Activate virtual Enviornment in Powershell:
- python -m venv .venv
- .venv/Scripts/Activate.ps1
- pip install -r requirements.txt

2. cd backend:
 - uvicorn main:app --reload --port 8000

3. cd frontend:
- streamlit run streamlit_app.py


