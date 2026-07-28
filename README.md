# AI-Powered Meeting Intelligence and Task Management System

## Overview

The **AI-Powered Meeting Intelligence and Task Management System** is a web application that automatically converts meeting audio recordings into structured meeting notes using Artificial Intelligence.

The application performs:

* 🎙️ Speech-to-text transcription
* 📝 AI-generated meeting summaries
* ✅ Task extraction
* 📅 Deadline identification
* 📆 Calendar integration
* 🔐 Secure user authentication
* 📚 Meeting history management

The system reduces manual effort by automatically documenting meetings and organizing action items.

---

# Features

* User Registration & Login (JWT Authentication)
* Upload meeting audio files
* AI-based speech transcription using Faster-Whisper
* Meeting summarization using BART Transformer
* Automatic task extraction
* Deadline detection using DateParser
* Calendar (.ics) file generation
* Meeting History
* Edit generated summaries
* Share summaries via Gmail
* Task status management

---

# Tech Stack

## Frontend

* React.js
* HTML
* CSS
* JavaScript
* Axios

## Backend

* FastAPI
* Python 3.14

## AI / NLP

* Faster-Whisper
* Hugging Face Transformers
* BART Model
* Regex
* DateParser

## Database

* SQLite

---

# Project Structure

```
meeting-backend/
│
├── main.py
├── requirements.txt
├── database/
├── routes/
├── services/
├── uploads/
└── ...

meeting_frontend/
│
├── src/
├── public/
├── package.json
└── ...
```

---

# Prerequisites

Install the following software before running the project:

* Python 3.14
* Node.js
* Visual Studio Code
* Git

---

# Verify Installation

Open Command Prompt or Terminal and run:

```bash
python --version
node -v
npm -v
```

---

# Backend Setup

## Step 1: Clone Backend Repository

```bash
git clone https://github.com/042sanjana/meeting-final.git
```

---

## Step 2: Navigate to the Project

```bash
cd meeting-final
```

---

## Step 3:
cd meeting-backend-main

## Step 4: Create a Virtual Environment

```bash
python -m venv venv
```

---

## Step 5: Activate the Virtual Environment

### Windows (Command Prompt)

```bash
venv\Scripts\activate
```

### Windows (PowerShell)

```bash
venv\Scripts\Activate.ps1
```

---

## Step 6: Install Required Python Packages

### Using requirements.txt (Recommended)

```bash
pip install -r requirements.txt
```

### If requirements.txt is unavailable

```bash
pip install fastapi
pip install uvicorn
pip install python-multipart
pip install transformers
pip install faster-whisper
pip install torch
pip install sentencepiece
pip install icalendar
pip install pydantic
pip install regex
pip install dateparser
```

---

## Step 7: Run the Backend Server

```bash
uvicorn main:app --reload
```

If successful, you should see:

```
Uvicorn running on http://127.0.0.1:8000
```

---

# API Documentation

FastAPI automatically generates Swagger documentation.

Open:

```
http://127.0.0.1:8000/docs
```

---

# Frontend Setup



---

## Step 1: Navigate to the Project

```bash
cd meeting_final
```

---
## Step 2: 
 cd meeting_frontend-main\(1)

## Step 3: Install Dependencies

```bash
npm install
```

---

## Step 4: Start the React Application

```bash
npm start
```

The frontend will start at:

```
http://localhost:3000
```

(or the port displayed in the terminal)

---

# Application Workflow

1. Register or log in to the application.
2. Upload a meeting audio file.
3. The backend transcribes the audio using Faster-Whisper.
4. The transcript is summarized using the BART Transformer model.
5. Tasks, deadlines, and priorities are extracted.
6. Calendar events are generated.
7. Users can:

   * View summaries
   * Edit summaries
   * Manage tasks
   * View meeting history
   * Share summaries via Gmail

---

# Technologies Used

| Technology        | Purpose            |
| ----------------- | ------------------ |
| React.js          | Frontend UI        |
| FastAPI           | Backend API        |
| SQLite            | Database           |
| Faster-Whisper    | Speech-to-Text     |
| Hugging Face BART | Text Summarization |
| Regex             | Task Extraction    |
| DateParser        | Deadline Detection |
| JWT               | Authentication     |

---

# Future Enhancements

* Speaker Diarization
* Multi-language Support
* Live Meeting Transcription
* Google Calendar Synchronization
* Outlook Integration
* Email Notifications
* Microsoft Teams Integration
* Slack Integration
* Analytics Dashboard
* Role-Based Access Control (RBAC)

---

# Contributors

**Sanjana Vinu**

---

# License

This project is developed for educational and learning purposes.
