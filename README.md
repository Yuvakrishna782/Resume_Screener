***AI Resume Screener***
*Project Overview*
The AI Resume Screener is a Streamlit-based application that automates the initial screening of job applicants by analyzing their resumes against predefined job role requirements. It uses NLP techniques to extract skills and calculate match scores, helping recruiters quickly identify top candidates.

*Features*
Automated Resume Scoring: Analyzes resumes and assigns match scores based on job-specific keywords

Multiple Job Roles: Predefined templates for Data Scientist, AI Engineer, Software Engineer, and DevOps roles

Interactive Dashboard: User-friendly interface with file upload, job selection, and results display

Exportable Results: Download shortlisted candidates as CSV

Skill Extraction: Identifies relevant skills from resume text using spaCy's NLP capabilities

Installation
Prerequisites
Python 3.8+

pip package manager
Troubleshooting
Ngrok Authentication Errors: Ensure you have a valid ngrok auth token if using ngrok for tunneling

CSV Format Issues: Verify your input file has the required columns ('application_name' and 'str_resume')

spaCy Model Errors: Reinstall the language model with python -m spacy download en_core_web_lg

Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your improvements.
