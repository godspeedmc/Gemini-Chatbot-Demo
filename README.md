# Gemini Chatbot Demo

A simple Streamlit-based chatbot demo that uses Google's Gemini API to generate responses in a conversational Q&A interface.

## Overview

This project demonstrates how to:

- configure a Google Gemini model in Python
- build a lightweight chat interface with Streamlit
- store chat history in session state
- send user prompts and stream responses back to the UI

## Features

- Interactive Q&A interface powered by Gemini
- Real-time streaming responses
- Session-based chat history
- Easy setup using environment variables
- Minimal dependencies for quick experimentation

## Tech Stack

- Python 3
- Streamlit
- Google Generative AI SDK
- python-dotenv

## Project Files

- `app.py` — Streamlit application and Gemini integration
- `requirements.txt` — Python dependencies
- `.env` — local environment variables (not committed in production repos)
- `README.md` — project documentation

## Prerequisites

Before running the app, make sure you have:

- Python 3.9+ installed
- A Google API key with access to Gemini models

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/godspeedmc/Gemini-Chatbot-Demo.git
   cd Gemini-Chatbot-Demo
   ```

2. Create and activate a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/macOS
   # or
   venv\Scripts\activate      # Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the project root and add your Gemini API key:

   ```env
   GOOGLE_API_KEY=your_api_key_here
   ```

## Run the App

```bash
streamlit run app.py
```

Then open the local URL shown by Streamlit in your browser.

## Example Usage

- Ask a factual question
- Request a summary or explanation
- Use the app as a simple demo for Gemini-powered chat interactions

## Notes

- The app uses the `models/gemini-2.0-flash` model.
- The generated responses are streamed chunk-by-chunk and displayed in the interface.
- Chat history is retained only while the session remains active in the browser.

## License

This project is provided for educational and demo purposes.
