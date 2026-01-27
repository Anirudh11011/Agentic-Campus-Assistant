# 🎓 Agentic Campus Assistant

An **AI-powered, agentic university assistant** built using **LangChain, Google Gemini, Whisper, ChromaDB, and Gradio**.  
This project is designed to assist **University of Texas at Arlington (UTA)** students by answering campus-related questions, booking study rooms, drafting and sending emails, and interacting through both text and voice.

---

## ✨ Features

- 🤖 **Agentic AI Assistant**
  - Tool-calling agent using LangChain
  - Maintains conversational memory
- 🔍 **University Knowledge Search**
  - Vector-based retrieval using ChromaDB
  - Sentence embeddings via HuggingFace
- 🎤 **Voice Input Support**
  - Speech-to-text using OpenAI Whisper
- 📧 **Email Automation**
  - Drafts emails
  - Sends emails only after user confirmation
- 📅 **Study Room Booking**
  - Collects required booking details
  - Prevents hallucinated or incomplete bookings
- 🌐 **Web & Location Tools**
  - Web scraping using BeautifulSoup
  - Distance and location lookup using Google Maps
- 💬 **Interactive UI**
  - Built using Gradio
  - Custom glass-morphism styled interface

---

## 🧱 Tech Stack

| Category | Technology |
|--------|-----------|
| LLM | Google Gemini (`gemini-2.5-flash`) |
| Agent Framework | LangChain |
| Speech-to-Text | OpenAI Whisper |
| Embeddings | all-MiniLM-L6-v2 |
| Vector Store | ChromaDB |
| UI | Gradio |
| Web Scraping | BeautifulSoup, Requests |
| Browser Automation | Playwright |
| Email | SMTP (Gmail SSL) |
| Maps | Google Maps API |

---

## 📁 Project Structure

