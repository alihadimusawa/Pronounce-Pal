# Gopal - Pronounce Pal

An interactive Streamlit app to practice and improve your pronunciation with real-time feedback and progress tracking using Google Sheets.

---

## Features

- Record your voice and get instant pronunciation feedback
- Track daily, weekly, monthly, and yearly progress
- Store user data and progress in Google Sheets
- Multi-language support for practice
- Clean, responsive UI with custom styling

---

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Google Cloud Project with Google Sheets and Drive APIs enabled
- A Google Service Account JSON key file

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/gopal-pronounce-pal.git
   cd gopal-pronounce-pal
Install dependencies:

bash
Salin
Edit
pip install -r requirements.txt
If requirements.txt is missing, install manually:

bash
Salin
Edit
pip install streamlit pandas numpy sounddevice scipy SpeechRecognition difflib gspread oauth2client
Google Cloud Setup
Go to Google Cloud Console.

Create a new project or select an existing one.

Enable the following APIs:

Google Sheets API

Google Drive API

Create a Service Account and download its JSON key file.

Share your Google Sheet with the Service Account email (found in the JSON file, under "client_email") and give it Editor access.

Setup Credentials
Place the downloaded JSON file in the project directory.

Rename it to credentials.json (or update your code with the correct filename).

Important: Do NOT commit credentials.json to GitHub.

Running the App
bash
Salin
Edit
streamlit run app.py
Replace app.py with your main script filename if different.

Security Tips
Add credentials.json to your .gitignore file to avoid uploading secrets to GitHub.

Consider using Streamlit Secrets for managing sensitive credentials securely if deploying on Streamlit Cloud.

Troubleshooting
SpreadsheetNotFound Error:
Make sure your Google Sheet name in the code matches exactly with your actual sheet name. Also confirm it’s shared with your service account email.

API Errors (403):
Double-check that both Google Sheets API and Google Drive API are enabled in your Google Cloud project.

License
MIT License © 2025 Your Name

