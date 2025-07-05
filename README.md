# 🎓 BacJourney - AI-Powered Learning for Algerian Students

**BacJourney** is a full-stack educational platform built to modernize how Algerian students prepare for their baccalaureate exams. It blends structured curriculum data with advanced AI interaction for precise, contextual answers—far beyond generic chatbots.

---

## 🔍 Problem Solved
Students often rely on outdated PDF documents. BacJourney replaces them with an interactive, trustworthy, and intelligent assistant based strictly on the official curriculum.

---

## 🏗️ Architecture Overview

- **Frontend**: `Next.js`, `React`, `TailwindCSS`
- **Backend**: `Custom RAG architecture`, `Google Gemini Pro API`
- **Auth**: `OAuth 2.0 with Google`, Tokens encrypted & stored via `httpOnly cookies`
- **Data**: PDF curriculum parsed into structured `JSON`
- **Visualization**: Gemini returns embedded `Plotly.js JSON` rendered as `SVG` charts

---

## 🔐 Security Implementation

- OAuth flow secured with encrypted tokens (backend + client)
- Scoped access to user’s private chat stored on Google Drive
- Real-time parsing + validation to avoid injection or stream-based exploits

---

## 🧠 AI Flow (RAG)

1. **Student logs in** (OAuth 2.0)
2. **User query submitted**
3. **RAG layer fetches relevant curriculum data**
4. **Structured context + question sent to Gemini API**
5. **Gemini responds with AI explanation + embedded Plotly JSON (if needed)**
6. **Frontend parses + renders diagram as live SVG**

---

## 🎬 Live Demo (No Code Exposed)
▶️ [Click here to watch the demo](https://bacjourney.vercel.app/)

---

## ⚙️ Project Highlights

- Self-architected RAG pipeline
- Custom prompt injection for curriculum-bound AI
- Real-time streaming parser for Plotly in Gemini
- CI/CD via Vercel + secured SSR rendering
- Privacy-focused: no student data stored locally

---

## 🚀 Tech Stack

| Layer       | Tools / Stack             |
|-------------|---------------------------|
| Frontend    | Next.js, React, Tailwind  |
| Backend     | Node.js (API), RAG Layer  |
| Auth        | Google OAuth 2.0          |
| AI Engine   | Google Gemini Pro         |
| Data        | JSON (from PDF parsing)   |
| Visualization | Plotly.js + SVG         |

---

## ❗ Why it Matters

BacJourney isn't a chatbot. It's an AI-based educational assistant grounded in curriculum, secure by design, and built for measurable impact.

---

## 🙋 About the Developer

👨‍💻 *Fekerine*  
Full-stack software engineer, security researcher, and AI systems developer.  
[Portfolio](https://fekerineamar.vercel.app/) | [LinkedIn]([f](https://www.linkedin.com/in/fekerine/)) | [Email](mailto:fekerineamar@gmail.com)

