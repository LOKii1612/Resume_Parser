🧠 Resume Parser and Matcher using NLP
=======================================
A Python-based intelligent resume analysis and job matching tool using Natural Language Processing (NLP). This tool extracts critical details from resumes (PDF/DOCX), analyzes job descriptions, calculates compatibility scores, and supports AI-driven queries using Anthropic's Claude AI.

🚀 Features
============
📄 Resume Parsing
------------------
Supports PDF and DOCX formats.

Extracts:

Full Name

Education Details

Technical and Soft Skills

Contact Information (Phone & Email)

📌 Job Description Analysis
============================
Extracts key responsibilities and required skills.

Performs keyword-based skill comparison.

Calculates match percentage for each candidate.

🤖 AI Integration (Claude AI)
=============================
Ask advanced questions like:

“Who is the best-fit candidate for this job?”

“Which candidate has the most relevant experience?”

🔍 Keyword Matching
--------------------
Uses spaCy and nltk for skill and keyword extraction.

Domain-specific keyword matching enabled via easy customization.

📦 Prerequisites
----------------
Python 3.7+

Install required libraries:

pip install anthropic docx2txt PyPDF2 spacy nltk
python -m spacy download en_core_web_sm

🛠️ Installation
===============
Clone the repository:

git clone https://github.com/<your-username>/resume-parser.git
cd resume-parser
Install dependencies:
pip install -r requirements.txt

⚙️ Usage
--------
Run the script:
python resume_parser.py
Upload files as prompted:

Job Description (PDF/DOCX)

One or More Resumes (PDF/DOCX)

View output:

Candidate name, skills, education, contact

Compatibility match percentage

Ask AI questions about the candidates

🧪 Sample Output
----------------
{
  "Name": "John Doe",
  "Education": ["B.Tech", "MBA"],
  "Skills": ["python", "data analysis", "sql"],
  "Mobile Number": "9876543210",
  "Email Addresses": ["johndoe@example.com"],
  "Match Percentage": 85.0
}
🤔 Example Query
----------------
Question: Who is the best candidate for this role?

Answer: John Doe with a match percentage of 85% is the most suitable candidate.

🔐 Important Notes
-------------------
Replace api_key in the script with your Anthropic Claude API Key.

Do NOT upload your API key to public repositories.

🛠️ Customization
----------------
To target specific industries:

Modify the predefined EDUCATION and SKILLS keyword lists in the script.

📌 Coming Soon
---------------
Resume ranking dashboard

Exportable PDF/CSV reports

Integration with job portals and ATS systems
