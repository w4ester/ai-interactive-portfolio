# AI Interactive Portfolio

An interactive portfolio website with AI chat capabilities, dynamic visualizations, and code examples.

## Features

- Interactive skill visualization
- AI-powered chat interface using Ollama
- Real-time code examples and execution
- Dynamic animations and transitions
- Dark/light theme support

## Setup

### Frontend

```bash
cd frontend
npm install
npm start
```

### Backend

```bash
cd backend
python -m venv venv
source venv/bin/activate  # or `venv\Scripts\activate` on Windows
pip install -r requirements.txt
uvicorn main:app --reload
```

### Ollama Setup

1. Install Ollama from https://ollama.ai/
2. Pull your preferred model:
```bash
ollama pull llama2
```

## Environment Variables

Create a `.env` file in both frontend and backend directories:

```env
# Frontend
REACT_APP_API_URL=http://localhost:8000

# Backend
OLLAMA_API_URL=http://localhost:11434
```

## Project Structure

```
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── InteractiveViz.js
│   │   │   ├── CodePreview.js
│   │   │   └── Chat.js
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
├── backend/
│   ├── main.py
│   └── requirements.txt
└── README.md
```