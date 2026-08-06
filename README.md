# OmniChat

OmniChat is an **agentic AI assistant** built with **Python, FastAPI, LangGraph, LangChain, Google Gemini, Tavily, ChromaDB, and SQLite**. It combines conversational AI, Retrieval-Augmented Generation (RAG), web search, persistent memory, document understanding, and voice input into a unified chat experience through a modern web interface.

---

## ✨ Features

- 💬 Real-time AI conversations powered by Google Gemini
- 🎙️ Voice input using the browser's Speech Recognition API
- 📄 Upload and chat with PDF, DOCX, TXT, Markdown, Python, and CSV files
- 🧠 Retrieval-Augmented Generation (RAG) over uploaded documents
- 🌐 Live web search using Tavily Search API
- 💾 Persistent conversation memory with SQLite
- ⚡ Token streaming for real-time AI responses
- 📚 Multiple chat sessions with conversation history
- 🎨 Responsive web interface built with HTML, CSS, and JavaScript

---

## 🏗️ Architecture

```
                    User
                      │
                      ▼
           HTML / CSS / JavaScript
                      │
                      ▼
               FastAPI Backend
                      │
                      ▼
              LangGraph Workflow
                      │
      ┌───────────────┼────────────────┐
      │               │                │
      ▼               ▼                ▼
 Google Gemini     Tavily Search      RAG
      │               │                │
      │               │          ChromaDB
      │               │                │
      └───────────────┼────────────────┘
                      │
                      ▼
             SQLite Conversation Memory
```

---

## 🚀 What OmniChat Can Do

- Answer general knowledge questions using Google Gemini
- Search the web for current information
- Chat with uploaded documents using Retrieval-Augmented Generation
- Remember previous conversations across chat sessions
- Accept voice input for hands-free interaction
- Stream responses token-by-token for a smooth user experience

---

## 🛠️ Tech Stack

### Backend
- Python
- FastAPI

### AI Frameworks
- LangGraph
- LangChain

### Language Model
- Google Gemini

### Search
- Tavily Search API

### Retrieval-Augmented Generation
- ChromaDB
- Vector Embeddings

### Database
- SQLite

### Frontend
- HTML
- CSS
- JavaScript
- Jinja2
- Web Speech API

---

## 📂 Supported File Types

- PDF
- DOCX
- TXT
- Markdown (.md)
- Python (.py)
- CSV

---

## 📁 Project Structure

```
OmniChat/
│
├── app.py
├── agent.py
├── rag.py
├── database.py
├── tools.py
├── templates/
│   └── index.html
├── uploads/
├── chroma_db/
├── data/
├── requirements.txt
├── README.md
└── .env
```

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/harshittt-21/OmniChat.git

cd OmniChat
```

Create a virtual environment

```bash
python -m venv .venv
```

Activate it

### Windows

```bash
.venv\Scripts\activate
```

### Linux / macOS

```bash
source .venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file.

```env
GOOGLE_API_KEY=YOUR_API_KEY
TAVILY_API_KEY=YOUR_API_KEY

# Optional
LANGSMITH_API_KEY=YOUR_API_KEY
LANGSMITH_TRACING=true
```

---

## ▶️ Running the Application

Start the FastAPI server

```bash
uvicorn app:app --reload
```

Open your browser

```
http://localhost:8000
```

---



## 🔮 Future Improvements

- Image understanding (multimodal support)
- Voice responses (Text-to-Speech)
- Authentication and user accounts
- Cloud database support
- Additional MCP tool integrations
- Docker deployment

---

---

## 📄 License

This project is licensed under the MIT License.
