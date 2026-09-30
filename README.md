# 🛡️ Sensitive Data Detection & Compliance Assistant

An AI-powered Streamlit application that detects sensitive information in documents, masks confidential data, classifies potential risks, and provides AI-generated compliance summaries and document-based Q&A.

## 📌 Project Overview

Handling sensitive information in documents manually can be time-consuming and error-prone.

This project provides a simple application where users can upload **PDF, TXT, or CSV files** and analyze their content for sensitive information such as personally identifiable information (PII).

The application combines **Python-based pattern detection** with **Google Gemini AI** to provide document analysis, risk insights, compliance summaries, and question answering.

## 🚀 Features

* 📄 Upload **PDF, TXT, and CSV** documents
* 🔍 Detect sensitive information using pattern-based detection
* 🛡️ Identify potentially confidential information
* 🎭 Mask detected sensitive information
* 📊 Generate AI-based compliance summaries
* 💬 Ask questions about uploaded documents
* 🤖 Google Gemini integration for AI analysis
* 🌐 Interactive Streamlit interface
* 🔐 API key stored using environment variables

## 🏗️ Project Structure

```text
sensitive_data/
│
├── app.py                 # Main Streamlit application
├── utils.py               # Document processing and AI functions
├── requirements.txt       # Python dependencies
├── .env                   # API key (DO NOT upload to GitHub)
├── .gitignore             # Files excluded from Git
└── README.md              # Project documentation
```

## ⚙️ Technologies Used

* **Python**
* **Streamlit**
* **Pandas**
* **NumPy**
* **PyPDF2**
* **Python-dotenv**
* **Google Gemini API**
* **Regular Expressions (Regex)**

## 🔄 How It Works

```text
User Uploads Document
        ↓
Extract Text
        ↓
Sensitive Data Detection
        ↓
Display Detected Information
        ↓
Mask Sensitive Information
        ↓
AI Risk & Compliance Analysis
        ↓
User Questions
        ↓
AI Generated Answers
```

## 🧠 Sensitive Data Detection

The application uses pattern-based detection to identify sensitive information from uploaded documents.

Examples include:

* Email addresses
* Phone numbers
* Other configurable sensitive data patterns

Detected information is displayed by category, and users can optionally view a masked version of the document.

## 🤖 AI Features

Google Gemini is used for:

### Compliance Summary

The application analyzes the uploaded document and generates an AI-based summary of potential risks and compliance concerns.

### Document Q&A

Users can ask questions about the uploaded document and receive AI-generated answers based on its content.

## 🔑 Environment Setup

Create a `.env` file in the project directory:

```env
GEMINI_API_KEY=your_gemini_api_key_here
```

**Important:** Never upload your `.env` file or API key to GitHub.

The `.gitignore` file should contain:

```text
.env
__pycache__/
*.pyc
.venv/
```

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/sensitive-data-compliance-assistant.git
```

Navigate to the project directory:

```bash
cd sensitive-data-compliance-assistant
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ Run the Application

Start the Streamlit application:

```bash
python -m streamlit run app.py
```

The application will open in your browser.

## 📋 Supported File Types

| File Type | Supported |
| --------- | --------- |
| PDF       | ✅         |
| TXT       | ✅         |
| CSV       | ✅         |

## 🔐 Security Note

This project is intended for demonstration and learning purposes.

Do not upload real confidential documents, passwords, financial information, medical records, or other highly sensitive data to an AI-powered application unless appropriate security, privacy, access-control, and data-retention measures are implemented.

Always keep API keys and secrets outside the source code.

## 🎯 Use Cases

* Document privacy checking
* PII detection
* Data compliance assistance
* Confidential document analysis
* AI-powered document Q&A
* Data security and compliance demonstrations

## 🔮 Future Improvements

* Add more sensitive-data patterns
* Support DOCX and Excel files
* Add advanced risk scoring
* Add role-based access control
* Add document-level encryption
* Add downloadable compliance reports
* Add database logging and audit trails
* Add support for additional LLM providers
* Improve PII detection using NLP/NER models

## 👨‍💻 Author

**Darshan Patil**

AI/ML & GEN AI Developer
Pune, Maharashtra, India

## ⭐ Project Purpose

This project demonstrates practical skills in:

* Python development
* Streamlit application development
* Data processing
* Regex-based information extraction
* AI/LLM integration
* Document analysis
* Data privacy concepts
* API integration
* Environment-variable management
