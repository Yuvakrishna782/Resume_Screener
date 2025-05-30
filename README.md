AI Resume Screener - GitHub README
Project Overview
The AI Resume Screener is a Streamlit-based application that automates the initial screening of job applicants by analyzing their resumes against predefined job role requirements. It uses NLP techniques to extract skills and calculate match scores, helping recruiters quickly identify top candidates.

Features
Automated Resume Scoring: Analyzes resumes and assigns match scores based on job-specific keywords

Multiple Job Roles: Predefined templates for Data Scientist, AI Engineer, Software Engineer, and DevOps roles

Interactive Dashboard: User-friendly interface with file upload, job selection, and results display

Exportable Results: Download shortlisted candidates as CSV

Skill Extraction: Identifies relevant skills from resume text using spaCy's NLP capabilities

Installation
Prerequisites
Python 3.8+

pip package manager

Setup
bash
# Clone the repository
git clone https://github.com/yourusername/ai-resume-screener.git
cd ai-resume-screener

# Create and activate virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt

# Download spaCy language model
python -m spacy download en_core_web_lg
Usage
Prepare your CSV file with applicant data (must include 'application_name' and 'str_resume' columns)

Run the application:

bash
streamlit run resume_screener.py
In the web interface:

Upload your CSV file

Select the job title you're screening for

Choose how many candidates to shortlist

Click "Analyze Resumes"

View and download results

File Structure
ai-resume-screener/
├── resume_screener.py      # Main application script
├── requirements.txt        # Python dependencies
├── README.md               # This file
└── sample_resumes.csv      # Example input file (optional)
Configuration
You can customize the job keywords by editing the JOB_KEYWORDS dictionary in resume_screener.py:

python
JOB_KEYWORDS = {
    "Data Scientist": ["python", "machine learning", "data analysis", "sql", "statistics"],
    "AI Engineer": ["python", "deep learning", "tensorflow", "pytorch", "nlp"],
    # Add/modify job roles as needed
}
Troubleshooting
Ngrok Authentication Errors: Ensure you have a valid ngrok auth token if using ngrok for tunneling

CSV Format Issues: Verify your input file has the required columns ('application_name' and 'str_resume')

spaCy Model Errors: Reinstall the language model with python -m spacy download en_core_web_lg

Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your improvements.

License
This project is licensed under the MIT License - see the LICENSE file for details.
