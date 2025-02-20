# AI Recruiter - Smart Interview System

## Overview
AI Recruiter is an intelligent interview system designed to streamline the hiring process by evaluating candidates through an interactive AI-driven interview session. The system analyzes candidates' responses, assesses their skills, and ensures authenticity.

## Features
- **Automated Interview**: Conducts an AI-driven Q&A session.
- **CV Analysis**: Extracts and processes text from PDF and TXT files.
- **AI Response Evaluation**: Detects potential AI-generated responses.
- **Score Assessment**: Provides an in-depth evaluation of candidates' responses.
- **User-Friendly UI**: Simple, intuitive web interface with a seamless user experience.

## Technologies Used
- **Backend**: Flask (Python), Flask-Session
- **Frontend**: HTML, Tailwind CSS, JavaScript
- **AI Models**: Deepseek-R1(G4f), Ollama
- **PDF Processing**: PyMuPDF

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Virtualenv (optional but recommended)

### Setup Instructions
```bash
# Clone the repository
git clone https://github.com/SreejiBR/RecruiterAI
cd Recruiter

# Install dependencies
pip install -r requirements.txt

Preferred IDE
PyCharm 2024.3.2 (Community Edition)
```

## Usage
1. Run the Flask server:
```bash
python app.py
```
2. Open your browser and navigate to `http://127.0.0.1:5000/`.
3. Upload a CV and enter job requirements.
4. Answer AI-generated interview questions.
5. Receive a score based on your performance.

## Choose Model

AI Recruiter is configured to use Deepseek-R1 with GPT4Free by default.

If you prefer to use a local LLM, follow these steps:

Install [Ollama](https://ollama.com/download) and the required [models](https://ollama.com/library).
Modify the app.py file, specifically the olla_request function, along with any other necessary files.
This allows you to customize the system to suit your preferred AI model.

## File Structure
```
AI-Recruiter/
│-- app.py             # Flask backend
│-- templates/         # HTML templates
  │-- index.html         # Frontend UI
│-- uploads/           # Uploaded CVs
│-- sessions/          # Flask session storage
│-- LICENSE            # License information
│-- README.md          # Project documentation
│-- CONTRIBUTING.md    # Contribution guidelines
```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contribution
Contributions are welcome! Please check [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

