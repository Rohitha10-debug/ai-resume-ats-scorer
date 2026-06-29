# ATS Resume Scorer

An AI-powered application that evaluates how well a resume aligns with a job description and provides actionable recommendations for improvement. The platform combines traditional NLP techniques, semantic similarity models, and LLM-generated feedback to deliver comprehensive ATS analysis.

## Features

* Resume upload support for PDF, DOC, and DOCX formats
* ATS compatibility scoring with detailed category-wise analysis
* Semantic matching between resumes and job descriptions
* Skill extraction and validation using NLP models
* Personalized improvement recommendations powered by LLMs
* User authentication with email/password and Google OAuth
* Analysis history storage and retrieval
* Exportable PDF reports

## Tech Stack

| Component                 | Technology                                                           |
| ------------------------- | -------------------------------------------------------------------- |
| Frontend                  | Streamlit                                                            |
| Backend                   | FastAPI (Python)                                                     |
| NLP                       | spaCy (`en_core_web_md`), Sentence Transformers (`all-MiniLM-L6-v2`) |
| LLM                       | Groq API (Llama 3)                                                   |
| Authentication & Database | Supabase                                                             |
| Report Generation         | WeasyPrint, Jinja2                                                   |

## Workflow

1. Upload a resume and provide a job description.
2. The system extracts skills, experience, and keywords from the resume.
3. Semantic similarity models compare the resume with the target role.
4. An ATS score and detailed breakdown are generated.
5. AI-powered recommendations suggest improvements to increase job alignment.

## Project Structure

```text
ai-resume-ats-scorer/
├── backend/                 # FastAPI services, APIs, and NLP logic
├── frontend/                # Streamlit interface and UI components
├── jupyter notebooks/       # Research and experimentation notebooks
├── requirements.txt         # Project dependencies
├── README.md
└── .gitignore
```

## Environment Variables

Create a `.env` file and configure the required API keys and service credentials.

Example:

```env
GROQ_API_KEY=your_groq_api_key
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
```

**Important:** Never commit `.env` files or `secrets.toml` files to version control.

## Future Enhancements

* Support for multiple resume templates
* Advanced keyword optimization suggestions
* Batch resume evaluation
* Resume benchmarking against industry standards
* MLOps pipeline for model monitoring and deployment

## Author

**Rohitha Panchamukhi M**
sss
