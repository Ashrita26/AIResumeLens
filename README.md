# AIResumeLens
AI-powered resume analyzer that compares a resume with a job description, identifies matching and missing skills, calculates job-fit percentage, evaluates resume quality, and provides personalized improvement suggestions using n8n and Google Gemini.
# 🤖 AI Resume & Job Match Analyzer

An AI-powered resume analysis and job matching tool built using **n8n** and **Google Gemini**.

The application allows a user to upload a resume PDF and provide a job description. The AI analyzes both and generates a structured report showing the candidate's job fit, matching skills, missing skills, additional skills, resume quality, problems, and improvement suggestions.

---

## 🚀 Live Demo

🔗 **Live Demo:** https://ashritadvns.app.n8n.cloud/form/02e08e17-bfe1-48b2-ad3a-d34e2ecad52b

Upload a resume PDF, enter a job description, and receive an AI-generated job-fit analysis.

---

## 📌 Project Overview

Job seekers often apply to multiple positions without knowing how closely their resume matches the requirements of a particular job.

This project solves that problem by automatically comparing a candidate's resume with a job description.

The system uses an AI agent to:

- Extract information from the uploaded resume
- Analyze the job description
- Identify required skills
- Identify candidate skills
- Compare both sets of skills
- Calculate an estimated job-match percentage
- Determine whether the candidate is a good fit
- Identify missing skills
- Identify additional skills
- Evaluate resume quality
- Detect potential resume problems
- Provide personalized improvement suggestions

---

## ✨ Features

### 📄 Resume Upload

Users can upload their resume as a PDF through an n8n form.

### 💼 Job Description Analysis

Users can paste the job description they want to apply for.

### 🔍 Skill Matching

The AI compares the skills mentioned in the resume with the skills required by the job description.

### ✅ Matching Skills

Shows skills that are present in both the resume and the job description.

### ❌ Missing Skills

Identifies important job requirements that are not clearly present in the resume.

### ➕ Additional Skills

Shows useful skills present in the resume that are not specifically required by the job description.

### 🎯 Job Match Percentage

The AI provides an estimated match percentage from 0–100%.

### 🟢 Fit Classification

The candidate is categorized as:

- **GOOD FIT** — 80–100%
- **PARTIAL FIT** — 60–79%
- **LOW FIT** — Below 60%

### 📊 Resume Quality Score

The AI evaluates the overall quality of the resume based on factors such as:

- Structure
- Clarity
- Relevance
- Professional presentation
- Skills
- Experience
- Project descriptions

### ⚠️ Resume Problem Detection

The system identifies potential weaknesses or areas that could reduce the effectiveness of the resume.

### 💡 Personalized Suggestions

The AI provides suggestions specifically related to the target job description.

### ⭐ Final Verdict

The system provides a short final recommendation explaining whether the candidate is a good fit for the role.

---

## 🏗️ Workflow Architecture

The workflow follows this process:

```text
User
  │
  ▼
n8n Form
  │
  ├── Resume PDF
  │
  └── Job Description
  │
  ▼
Extract From File
  │
  ▼
AI Agent
  │
  ├── Resume Analysis
  ├── Job Description Analysis
  ├── Skill Matching
  ├── Missing Skills
  ├── Additional Skills
  ├── Job Match Percentage
  ▼
Form Ending
  │
  ▼
Job Fit Report

🔐 Security

This repository does not contain API keys or private credentials.

Before sharing an n8n workflow publicly:

Remove API keys
Remove authentication tokens
Remove passwords
Remove private webhook URLs
Avoid uploading personal resumes
Avoid uploading private candidate information

⚠️ Limitations

The job-match percentage is an AI-generated estimate, not a scientifically validated hiring score.

The system may occasionally:

Misinterpret skills
Miss equivalent skills
Misunderstand job requirements
Make incorrect assumptions
Give an imperfect match percentage

Users should review the AI recommendations before making career decisions.

🔮 Future Improvements

Possible future improvements include:

ATS compatibility scoring
Resume keyword optimization
Multiple job-description comparison
Resume section-by-section analysis
Better skill normalization
LinkedIn profile analysis
Job recommendation system
Resume rewriting
Cover-letter generation
Interactive dashboard
Industry-specific scoring
Better structured JSON output
Automated resume improvement
