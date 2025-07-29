# 📌 Skill2Project_Recommender_System
*A system that reads your resume and recommends the best-fit projects using SQL + Python.*

## 🧠 Project Description

**Skill2Project Recommender System** is a personalized project suggestion tool designed to help individuals, especially beginners and job seekers, discover the most relevant and impactful projects based on their actual skill sets. This system extracts technical skills from a user’s resume (PDF/Text) and matches them against a predefined database of real-world projects with their required tech stack. It then recommends projects that align best with the user’s existing capabilities.

Think of it as a smart assistant that reads your resume and answers:  
👉 *“Based on what you know, here are the projects you should build next!”*

## 💡 Why This Project?

As someone starting in Data Analytics, I often found myself asking:  
*"I know SQL and Python—but what project should I build to prove that?"*
Most students and job seekers face this gap between *what they’ve learned* and *what they can build*. Rather than downloading random project datasets, this tool gives **targeted** project recommendations based on your actual resume.

- ✅ Helps in project-based portfolio building  
- ✅ Saves time choosing what to work on  
- ✅ Aligns learning efforts with career goals  
- ✅ Makes your resume + GitHub more personalized and impactful

## 📂 Dataset Used

This project doesn’t rely on public Kaggle datasets.  
It uses **real resumes** (initially my own, and then anonymized samples from my friends from different backgrounds) to:

- Extract skills using Python-based parsing  
- Simulate real-life hiring scenarios for project matching  
- Ensure the recommendations are grounded in actual profiles, not pre-cleaned datasets  

This gave me **hands-on experience** in data extraction, text cleaning, and working with semi-structured data: core skills for any Data Analyst.

## 🛠 Tech Stack

| Tool/Library             | Purpose                                                  |
|--------------------------|----------------------------------------------------------|
| **Python**               | Main scripting and data flow                             |
| `spaCy`                  | Extracting skills and keywords from text                 |
| `PyMuPDF`                | Reading and extracting raw text from PDFs                |
| `re` (Regex)             | Custom rule-based parsing and cleaning                   |
| **Pandas**               | Structuring and cleaning skill data                      |
| **MySQL**                | Creating and querying resume and project tables          |
| `mysql-connector-python` | Connecting Python to MySQL                               |
| *(Optional)* `Matplotlib`| Visualizing skill gaps or project coverage               |


## 🧩 System Design

This project follows an end-to-end data flow that simulates how companies might match candidate skills with project needs.

### 🔸 MySQL Tables Designed

| Table Name            | Purpose                                                        |
|-----------------------|----------------------------------------------------------------|
| resume_skills       | Stores emp_id, resume_name, and extracted list of skills         |
| projects            | Contains project_id, project_name, and required skill set        |
| recommended_projects| Maps emp_id to best-fit project_id based on skill overlap logic  |

These normalized tables helped simulate a realistic relational schema used in hiring platforms or HR tools.

## 🧠 What I Learned

This project wasn’t just a technical build;  it was an **end-to-end simulation of a real-world data analyst task**. Here’s what it helped me grow in:

### 🔍 Real-World Data Handling
- I worked with **semi-structured data** (real resumes, not pre-cleaned CSVs) — a common scenario in data jobs.
- Applied **text extraction and NLP** to transform raw PDFs into actionable insights.

### 🧠 Skill Extraction Logic
- Built a hybrid approach using **spaCy** and **Regex** for more accurate keyword recognition.
- Handled variations in skill names (e.g., “Python 3” vs “Python”) using pattern matching.

### 🗃️ Database Design & SQL Thinking
- Designed normalized MySQL tables to structure resumes, skills, and project mappings.
- Used **SQL joins and filtering logic** to power project recommendations, replicating what companies do with matching engines.

### 🐼 Pandas for Structuring and Cleaning
- Leveraged Pandas to **transform unstructured resume content** into clean DataFrames ready for storage and analysis.
- Practiced real-time debugging and formatting while preparing it for MySQL ingestion.

### 🔁 End-to-End Integration
- Connected multiple tech stacks: PDF parsing ➝ NLP ➝ Pandas ➝ SQL ➝ Recommendation logic.
- This helped me **understand data pipelines** and how tools work together in production.

### 🧩 Project Thinking & Recruiter Empathy
- I didn’t just build: I built **for the end-user**, imagining how recruiters think while filtering resumes.
- Practiced **thinking like a hiring system**: what matters in a skill, what makes a candidate fit, and how to automate relevance.

### ✅ Why This Makes Me Job-Ready
- I didn’t use a Kaggle dataset.
- I built a real tool using real profiles to **solve a hiring problem** — exactly the kind of initiative recruiters want.

This shows I can:
- **Understand messy business data**
- Build full pipelines using Python + SQL
- Think from a **product and problem-solving perspective**, not just code.





