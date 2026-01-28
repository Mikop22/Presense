# Spurhacks2025
---

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [Demo Quick Start](#demo-quick-start)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Authors](#authors)

---

## Project Overview

We are an AI B2B SAAS helping small and medium sized-businesses to reduce HR interviewing and new recruit onboarding costs, by using a combination of LLM and CV in analyzing users' speeches.

## Features
- AI-powered backend using Google GenAI, OpenAI
- Modern, responsive frontend with React and Tailwind CSS
- Modular code structure for easy development

## Tech Stack

**Backend:**
- Python
- FastAPI 
- google-genai
- OpenAI
- Google Gemini

**Frontend:**
- React
- Tailwind CSS
- TensorFlow.js

---

## Getting Started

### Prerequisites

Before running the application, ensure you have the following installed:

1. **Python 3.9+** - [Download Python](https://www.python.org/downloads/)
2. **Node.js 18+** - [Download Node.js](https://nodejs.org/)
3. **FFmpeg** - Required for audio/video processing
   - **macOS**: `brew install ffmpeg`
   - **Ubuntu/Debian**: `sudo apt install ffmpeg`
   - **Windows**: [Download FFmpeg](https://ffmpeg.org/download.html) and add to PATH

4. **API Keys** (required):
   - **Gemini API Key**: Get from [Google AI Studio](https://aistudio.google.com/app/apikeys)
   - **LemonFox API Key**: Get from [LemonFox](https://lemonfox.ai/) (used for audio transcription)

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. (Recommended) Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Set up environment variables:
   ```bash
   cp .env.example .env
   # Edit .env and add your API keys:
   # - GEMINI_API_KEY: from https://aistudio.google.com/app/apikeys
   # - OPENAI_API: from https://lemonfox.ai/
   ```
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Run the backend server:
   ```bash
   python main.py
   ```
   The backend will start at `http://localhost:8000`

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run start
   ```
   The frontend will start at `http://localhost:3000`

---

## Demo Quick Start

Follow these steps to quickly get the application running for a demo:

### Step 1: Get API Keys
1. Go to [Google AI Studio](https://aistudio.google.com/app/apikeys) and create a Gemini API key
2. Go to [LemonFox](https://lemonfox.ai/) and create an API key for transcription

### Step 2: Start Backend
```bash
cd backend
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
cp .env.example .env
# Edit .env and add your GEMINI_API_KEY and OPENAI_API keys
pip install -r requirements.txt
python main.py
```

### Step 3: Start Frontend (in a new terminal)
```bash
cd frontend
npm install
npm run start
```

### Step 4: Run the Demo
1. Open your browser to `http://localhost:3000`
2. Click "Try Demo"
3. Allow camera/microphone access when prompted
4. Click "Start Recording" and give a short speech
5. Click "Stop Recording" when done
6. Click "Analyze Speech" to see AI-powered feedback

### Troubleshooting
- **Camera not working**: Ensure your browser has camera/microphone permissions
- **Backend errors**: Check that both API keys are correctly set in `.env`
- **FFmpeg errors**: Verify FFmpeg is installed and accessible via command line

---

## License

Refer to our LICENSE file

---
