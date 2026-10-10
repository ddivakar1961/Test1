# ReplyMate AI — Groq WhatsApp Reply Assistant

A polished local web dashboard for testing Groq-generated WhatsApp reply drafts. **This starter project does not connect to WhatsApp, read WhatsApp chats, or send messages.** It is a safe frontend/backend foundation to test replies first.

## Requirements
- Python 3.10+
- VS Code (optional but recommended)
- A Groq API key from https://console.groq.com/

## Run in VS Code

1. Extract the ZIP and open the `groq_whatsapp_ai_bot` folder in VS Code.
2. Open Terminal → New Terminal.
3. Create a virtual environment:

   Windows:
   ```powershell
   py -m venv .venv
   .venv\Scripts\Activate.ps1
   ```

   macOS/Linux:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

4. Install packages:
   ```bash
   python -m pip install -r requirements.txt
   ```
5. Copy `.env.example` to `.env` and replace the placeholder with your Groq API key.
6. Start the app:
   ```bash
   python app.py
   ```
7. Open http://127.0.0.1:5000 in your browser.

## Security
- Never share your Groq API key or commit `.env` to GitHub.
- Do not paste passwords, WhatsApp verification codes, or sensitive personal data into the demo.
- AI replies can be wrong. Review drafts before sending.
- Do not use unofficial tools that ask for WhatsApp Web session tokens or QR/login credentials.

## WhatsApp integration is not included
To receive/send real messages, set up a supported official WhatsApp Business Platform integration and webhook. Eligibility for using the same number with the WhatsApp Business app and API varies; confirm current official requirements before changing your number/account:
https://developers.facebook.com/docs/whatsapp/cloud-api/overview

This demo intentionally does not send messages or pretend WhatsApp is connected.
