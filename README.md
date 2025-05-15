# Email Automation Bot

## Overview
This project is a Python-based email automation bot that reads data from a Google Sheet and sends personalized emails to recipients using Gmail's SMTP server. It’s designed to automate repetitive tasks like sending payment reminders or newsletters, saving time for businesses.

## Features
- Reads email addresses and messages from a Google Sheet using the Google Sheets API.
- Sends emails securely via Gmail with an App Password.
- Uses environment variables to protect sensitive information.
- Includes error handling for robust performance.

## Technologies Used
- **Python**: Core programming language.
- **gspread**: For interacting with Google Sheets.
- **smtplib**: For sending emails via Gmail.
- **python-dotenv**: For secure management of credentials.
- **Google Sheets API & Google Drive API**: For accessing spreadsheet data.

## Setup Instructions
1. **Clone the Repository** (once uploaded to GitHub):
   ```bash
   git clone <[your-repo-url](https://github.com/QBK13/EmailBotProject.git)>
   cd EmailBotProject
2. **Install Dependencies:**
pip install gspread oauth2client python-dotenv
3. **Set Up Google Cloud**
Set Up Google Cloud:
Create a Google Cloud project and enable the Google Sheets and Drive APIs.
Generate a service account key (credentials.json).
Share your Google Sheet with the service account email.
4. **Configure Gmail:**
Enable 2-Step Verification and generate an App Password for Gmail.
5. **Create a .env File:**
SENDER_EMAIL=your.email@gmail.com
APP_PASSWORD=your_app_password
6. **Run the Script:**
python email_bot.py
## **Security Features**
Uses an App Password instead of the main Gmail password.
Stores sensitive data in a .env file, excluded from version control via .gitignore.
Employs SMTP_SSL for secure email transmission.
## **Future Improvements**
Add a scheduling feature to send emails at specific times.
Support for email templates with HTML formatting.
Integration with other APIs (e.g., CRM systems).
