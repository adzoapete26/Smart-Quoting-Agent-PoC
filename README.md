# Veracity Insurance — Smart Quoting Agent (PoC)

This Proof of Concept demonstrates an automated Smart Quoting workflow that allows users to upload a Certificate of Insurance (COI) and instantly receive an eligibility decision and competitive quote based on internal underwriting rules.

## Live Demo
(Insert your Streamlit Cloud link here)
Example: https://scriptpy-bezxevvwtzdo2xu7wgwytq.streamlit.app/

## Features
- Upload COI PDF and automatically extract:
  - General Aggregate limit
  - Policy Expiration Date
  - Current Premium
- Apply underwriting rules:
  - Decline if General Aggregate > $2,000,000
  - Decline if Expiration < 30 days
- Calculate competitive price (10% lower than current premium)
- Display automated approval or decline response

## Tech Stack
| Component | Technology |
|-----------|------------|
| Front End | Streamlit |
| Document Extraction | PyPDF2 |
| Rules Engine | Python logic |
| Deployment | Streamlit Cloud / GitHub |

## 📂 Project Structure
smart-quoting-poc/
├── script.py # Main app
├── requirements.txt
├── README.md
└── architecture-diagram.png 

## 🔧 Installation (Run locally)
```bash
pip install -r requirements.txt
streamlit run script.py

