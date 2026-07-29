# AI-Powered Meeting Intelligence and Task Management System

## Overview

The **AI-Powered Meeting Intelligence and Task Management System** is a web application that automatically converts meeting audio recordings into structured meeting notes using Artificial Intelligence.

The system helps users save time by automatically documenting meetings, generating summaries, extracting action items, identifying deadlines, and organizing tasks efficiently.

The application performs:

- 🎙️ Speech-to-Text Transcription
- 📝 AI-Generated Meeting Summaries
- ✅ Automatic Task Extraction
- 📅 Deadline Identification
- 📆 Calendar (.ics) Generation
- 🔐 Secure User Authentication
- 📚 Meeting History Management

---

# Features

- User Registration & Login (JWT Authentication)
- Upload Meeting Audio Files
- AI-Based Speech Transcription using Faster-Whisper
- AI Meeting Summarization using Hugging Face BART
- Automatic Task Extraction
- Deadline Detection using DateParser
- Calendar (.ics) File Generation
- Meeting History
- Edit Generated Summaries
- Share Summaries via Gmail
- Task Status Management

---

# Tech Stack

## Frontend

- React.js
- HTML
- CSS
- JavaScript
- Axios

## Backend

- FastAPI
- Python 3.14

## AI / NLP

- Faster-Whisper
- Hugging Face Transformers
- BART Transformer Model
- Regex
- DateParser

## Database

- SQLite

---

# Project Structure

```text
meeting-final/
│
├── meeting-backend-main/
│   ├── database/
│   ├── routes/
│   ├── services/
│   ├── uploads/
│   ├── main.py
│   ├── requirements.txt
│   └── ...
│
├── meeting_frontend-main/
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── ...
│
└── README.md
```

---

# Prerequisites

Install the following software before running the project.

- Python 3.14
- Node.js
- npm
- Git
- Visual Studio Code (Recommended)

---

# Verify Installation

Open Command Prompt or Terminal and run:

```bash
python --version
node -v
npm -v
```

Example Output

```text
Python 3.14.x
v22.x.x
10.x.x
```

---

# Backend Setup

## Step 1: Clone the Repository

```bash
git clone https://github.com/042sanjana/meeting-final.git
```

---

## Step 2: Navigate to the Project Folder

```bash
cd meeting-final
```

---

## Step 3: Navigate to Backend

```bash
cd meeting-backend-main/meeting-backend-main
```

---

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

### Linux / macOS

```bash
source venv/bin/activate
```

---

## Step 6: Install Required Packages

### Recommended

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

## Step 7: Start the Backend Server

```bash
uvicorn main:app --reload
```

If everything is configured correctly, you should see:

```text
INFO:     Uvicorn running on http://127.0.0.1:8000
```

---

# Backend API Documentation

FastAPI automatically generates interactive API documentation.

Open your browser and visit:

```text
http://127.0.0.1:8000/docs
```

Swagger UI allows you to test every API endpoint directly from the browser.

---

# Frontend Setup

## Step 1: Open a New Terminal

Navigate back to the project root.

```bash
cd meeting-final
```

---

## Step 2: Navigate to Frontend

```bash
cd meeting_frontend-main/meeting_frontend-main
```

---

## Step 3: Install Node Modules

```bash
npm install
```

---

## Step 4: Start the React Application

```bash
npm start
```

The frontend will launch at:

```text
http://localhost:3000
```

(or another available port displayed in the terminal.)

---

# Complete Application Workflow

```text
                User
                  │
                  ▼
          Login / Register
                  │
                  ▼
        Upload Audio Recording
                  │
                  ▼
        Faster-Whisper Model
        (Speech-to-Text)
                  │
                  ▼
          Meeting Transcript
                  │
                  ▼
       BART Transformer Model
        (Text Summarization)
                  │
                  ▼
        AI Generated Summary
                  │
      ┌───────────┴────────────┐
      ▼                        ▼
 Task Extraction        Deadline Detection
      │                        │
      └───────────┬────────────┘
                  ▼
          Calendar (.ics)
                  │
                  ▼
        Store in SQLite Database
                  │
                  ▼
          Display in React UI
                  │
                  ▼
    Edit • Share • Search • History
```

---

# Application Workflow

1. Register or log in.
2. Upload a meeting audio recording.
3. Faster-Whisper converts speech into text.
4. The transcript is summarized using the Hugging Face BART model.
5. AI extracts tasks from the summary.
6. DateParser identifies deadlines.
7. Calendar events are generated as `.ics` files.
8. Meeting information is stored in SQLite.
9. Users can:
   - View meeting summaries
   - Edit summaries
   - Manage extracted tasks
   - Track meeting history
   - Share summaries via Gmail

---

# Technologies Used

| Technology | Purpose |
|------------|---------|
| React.js | Frontend User Interface |
| FastAPI | Backend REST API |
| SQLite | Database |
| Faster-Whisper | Speech-to-Text |
| Hugging Face BART | Text Summarization |
| Regex | Task Extraction |
| DateParser | Deadline Detection |
| JWT | Authentication |
| Axios | API Communication |

---

# Major Modules

### Authentication Module

- User Registration
- User Login
- JWT Authentication

---

### Audio Processing Module

- Upload Audio
- Speech-to-Text using Faster-Whisper

---

### AI Processing Module

- Meeting Summarization
- Task Extraction
- Deadline Identification

---

### Task Management Module

- View Tasks
- Update Task Status
- Edit Summaries

---

### Calendar Module

- Generate `.ics` Calendar Files
- Download Calendar Events

---

### Meeting History Module

- Store Meetings
- Search Previous Meetings
- View Complete Meeting History

---

# Future Enhancements

- Speaker Diarization
- Multi-Language Support
- Live Meeting Transcription
- Google Calendar Integration
- Outlook Calendar Integration
- Microsoft Teams Integration
- Slack Integration
- Email Notifications
- Analytics Dashboard
- Role-Based Access Control (RBAC)

---

# Contributors

**Sanjana Vinu**

---

# License

This project is developed for educational and learning purposes.

---
