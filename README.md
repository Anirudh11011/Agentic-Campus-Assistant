# 🎓 Agentic Campus Assistant

## 📌 Project Overview

**Agentic Campus Assistant** is an AI-powered conversational assistant designed to help university students and staff with campus-related tasks using natural language and voice input.  
The system combines **LLM reasoning, tool-based agents, retrieval-augmented generation (RAG), speech-to-text**, and a **web-based chat interface** to simulate an intelligent campus help desk.

The assistant can:
- Answer campus and university-related questions
- Search and retrieve relevant information from stored knowledge
- Transcribe spoken audio queries into text
- Perform task-oriented actions such as:
  - Drafting emails
  - Sending emails after user approval
  - Booking study rooms
  - Searching campus resources
  - Providing distance/location-related information
- Maintain conversational context across interactions

This project demonstrates an **agentic AI workflow**, where an LLM dynamically decides when and how to use tools to fulfill user requests.

---

## 🧠 Core Concepts & Techniques Used

- Agentic AI (Tool-using LLM agents)
- Retrieval-Augmented Generation (RAG)
- Conversational Memory Management
- Speech-to-Text Processing
- Vector Similarity Search
- Web Scraping for Information Retrieval
- Human-in-the-loop Email Approval
- Multimodal Interaction (Text + Voice)

---

## 🧩 System Architecture (High-Level)

1. **User Interface** (Gradio Web App)
2. **Speech Input** (Optional Audio)
3. **Speech-to-Text** (Whisper)
4. **LLM Reasoning Engine** (Gemini via LangChain)
5. **Tool Invocation Layer**
6. **Knowledge Retrieval** (Vector Database)
7. **Action Execution** (Email, Search, Booking, etc.)
8. **Response Generation**

---

## 🛠️ Tech Stack & Tools Used

### 🔹 Programming Language
- **Python**

---

### 🔹 Large Language Models (LLMs)
- **Google Gemini 2.5 Flash**
  - Accessed via `langchain-google-genai`
  - Used for reasoning, tool selection, and response generation

---

### 🔹 Agent Framework & Orchestration
- **LangChain**
  - Agent creation and execution
  - Tool binding and invocation
  - Prompt templating
  - Chat history and memory handling
- **LangChain Community Modules**
- **LangChain Tools API**

---

### 🔹 Embeddings & Semantic Search
- **Hugging Face Sentence Transformers**
  - Model: `all-MiniLM-L6-v2`
- **HuggingFaceEmbeddings**
- **ChromaDB**
  - Vector database for storing and retrieving university-related information
  - Used for RAG (Retrieval-Augmented Generation)

---

### 🔹 Speech & Audio Processing
- **OpenAI Whisper**
  - Automatic speech recognition (ASR)
  - Converts audio queries into text
- **FFmpeg**
  - Audio processing dependency for Whisper

---

### 🔹 Web Interface
- **Gradio**
  - Interactive web-based chat UI
  - Supports text and audio inputs
  - Displays conversational responses

---

### 🔹 Web Search & Scraping
- **Requests**
- **BeautifulSoup (bs4)**
  - HTML parsing and content extraction
- **Playwright**
  - Browser automation for dynamic web content
  - Chromium browser engine

---

### 🔹 Email & Communication Tools
- Custom LangChain tools for:
  - Email drafting
  - Email sending (only after explicit user approval)
- Human-in-the-loop validation for sensitive actions

---

### 🔹 Conversational Memory
- **ChatMessageHistory**
- **HumanMessage / AIMessage**
- Maintains multi-turn conversational context

---

### 🔹 Additional Utilities & Libraries
- **OS**
- **Environment Variable Handling**
- **Custom Python Functions as Tools**

---

## 🤖 Agent Capabilities

The assistant dynamically decides when to:
- Answer directly using the LLM
- Retrieve information from the vector database
- Call external tools
- Ask for user confirmation before executing sensitive actions

This makes the assistant **context-aware, safe, and action-capable**.

---

## 🎯 Use Cases

- Campus information assistant
- AI-powered student help desk
- Demonstration of agentic AI systems
- RAG-based chatbot for institutions
- Voice-enabled AI assistant prototype

---

## 🚀 Key Highlights

- Fully agent-based AI system
- Combines LLMs + tools + memory
- Voice and text interaction support
- Safe execution with user approvals
- Modular and extensible design

---

## 📄 License

This project is intended for educational and experimental purposes.
