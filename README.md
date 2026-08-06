# agentic_chatbot


**agentic AI chatbot** built with  **Python, FastAPI, LangGraph, LangChain, Google Gemini, Tavily, ChromaDB, and SQLite** .

It supports real-time streaming chat, document uploads, retrieval-augmented generation (RAG), web search, conversation memory, and a simple web UI.

---

## Features

* Chat with an AI agent powered by Google Gemini
* Stream responses in real time
* Upload documents such as PDF, DOCX, TXT, MD, PY, and CSV
* Use uploaded files as context through RAG
* Search the web with Tavily for current information
* Store and recall conversation history
* Simple FastAPI-based web interface
* Docker-ready deployment
* AWS CI/CD support using GitHub Actions, ECR, and EC2

---

## Project Overview

This project combines:

* **FastAPI** for the backend server and API endpoints
* **Jinja2** for rendering the frontend UI
* **LangGraph** for agent orchestration
* **LangChain** for tools, messages, and RAG workflow
* **Google Gemini** as the LLM provider
* **Tavily** for web search
* **ChromaDB** for vector search over uploaded documents
* **SQLite** for conversation and persistence
* **Docker** for containerized deployment

---

## Prerequisites

Make sure you have the following installed:

* Python 3.11
* Git
* Google API key for Gemini
* Tavily API key for web search
