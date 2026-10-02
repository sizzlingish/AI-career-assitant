# 💼 CareerOps AI

> Your AI-powered career operations team for job applications and interview preparation.

## 🚀 Overview

CareerOps AI is a multi-agent AI career assistant that helps candidates prepare for job opportunities.

The system analyzes a job description and CV, matches the candidate's qualifications with the job requirements, creates customized application materials, prepares interview questions, and reviews the final application package.

## 🤖 AI Agents

CareerOps AI uses specialized AI agents:

1. 🧠 **Manager Agent** — Coordinates the career workflow
2. 🔎 **Job Analyst Agent** — Analyzes job descriptions
3. 📄 **CV Agent** — Analyzes candidate CVs
4. 🔗 **Matching Agent** — Matches CV qualifications with job requirements
5. ✍️ **Application Agent** — Creates customized application materials
6. 🎤 **Interview Agent** — Prepares interview questions
7. 🧐 **Reviewer Agent** — Reviews the final career package

## 🔄 Workflow

```text
User
  ↓
Upload CV + Job Description
  ↓
CareerOps AI
  ↓
Job Analysis
  ↓
CV Analysis
  ↓
Job ↔ CV Matching
  ↓
Application Generation
  ↓
Interview Preparation
  ↓
Final Review
  ↓
Career Application Package
```

## ⚙️ Setup

```bash
pip install -r requirements.txt
cp .env.example .env      # then add your XAI_API_KEY
streamlit run app.py
```

CareerOps AI runs on **Grok (xAI)**. Get an API key at https://console.x.ai.
On Streamlit Cloud, add `XAI_API_KEY` under *Secrets*. Set `XAI_MODEL` to switch models (default: `grok-4.7`).

## 📁 Project Structure

```text
CareerOps-AI/
├── app.py
├── requirements.txt
├── .env.example
├── .streamlit/secrets.toml.example
└── careerops/
    ├── config.py    # Grok LLM setup
    ├── agents.py
    ├── tasks.py
    ├── crew.py
    ├── prompts.py
    ├── tools.py
    └── utils.py     # CV text extraction
```
