
# PolicyPulse – Automated Policy & PII Compliance Scanner

> A lightweight Streamlit app for detecting internal policy violations and sensitive personal data in emails or documents.

---

## Overview

**PolicyPulse** helps organizations automatically identify potential compliance breaches in text content such as emails or uploaded files.

The system uses a **rule-based scanning engine** to flag:

* **Restricted terms** — e.g., "confidential", "salary", "internal use only"
* **Personally Identifiable Information (PII)** — e.g., phone numbers, email addresses, Social Security numbers

* ## Project Structure

PolicyPulse/
├── app.py
├── rules/
│   └── rules.json
├── data/
│   └── scan_results.json
├── sample_emails.json    
├── utils/
│   ├── rule_engine.py
│   ├── email_loader.py
│   └── scan_manager.py
├── test_rules.py
│   
├── README.md
└── prompt_log.md

**Built with:**

* Python
* Streamlit (for interactive UI)
* spaCy + Regex (for NLP and pattern matching)
* Fully open-source libraries

---

## Features

* Browse and scan a sample email inbox
* Highlight flagged terms with details on violations
* Maintain scan history for review
* Detect both keyword- and regex-based patterns
* Unit test coverage for scanning logic
* Well-documented with AI-assisted development prompts

---

## Installation & Usage

1. **Install dependencies:**

   
   pip install -r requirements.txt
   

2. **Run the application:**

   
   streamlit run app.py
  

3. **Run tests:**

   
   python -m unittest discover tests
  

---

## Sample Email Format

```json
{
    "id": "email_008",
    "subject": "Job Application",
    "body": "Candidate applied with contact 9123456789. Resume attached."
}
```

---

## Development Notes / AI Prompt Log

* Developed a rule engine combining regex and forbidden terms
* Created a Streamlit-based interface for real-time scanning
* Implemented unit tests to ensure rule accuracy


