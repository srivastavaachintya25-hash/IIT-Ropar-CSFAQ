
# 🏛️ Crowd Sourcing FAQ & AI Assistant Portal
### Official FAQ & Information Hub — IIT Ropar

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-Vercel-black?style=for-the-badge)](https://iit-ropar-seven.vercel.app)
[![Backend](https://img.shields.io/badge/⚙️_API-Render-46E3B7?style=for-the-badge)](https://vicharanashala-internship.onrender.com)
[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react)](https://react.dev)
[![FastAPI](https://img.shields.io/badge/FastAPI-Python-009688?style=for-the-badge&logo=fastapi)](https://fastapi.tiangolo.com)
[![Gemini](https://img.shields.io/badge/Gemini_2.0_Flash-AI-4285F4?style=for-the-badge&logo=google)](https://ai.google.dev)

</div>

---

## 🌐 Live Website

**Frontend:** https://iit-ropar-seven.vercel.app

**Backend API:** https://iit-ropar.onrender.com

---

## 🖼️ Screenshots
<img width="1095" height="620" alt="Screenshot 2026-06-20 114512" src="https://github.com/user-attachments/assets/8516c3ca-669e-49fd-882c-7573919dda44" />
<img width="1082" height="615" alt="Screenshot 2026-06-20 114615" src="https://github.com/user-attachments/assets/76b06219-4cf2-45cc-a29f-40de96aee764" />
<img width="1079" height="615" alt="Screenshot 2026-06-20 114700" src="https://github.com/user-attachments/assets/21d3244b-cc17-42b0-b994-8875df1f5f77" />

---
## 📌 About the Project

The Crowd Sourcing FAQ & AI Assistant Portal is a full-stack web application developed as part of the Vicharanashala Internship Programme 2026 at IIT Ropar, an open-source initiative led by the Lab of Prof. Sudarshan Iyengar.

The platform serves as a centralized knowledge and support hub for interns, providing instant access to internship-related information through an interactive FAQ system and an AI-powered virtual assistant.

Designed to reduce repetitive queries and improve information accessibility, the portal combines crowd-sourced knowledge, multilingual support, and generative AI to deliver a modern self-service experience.

The portal provides:

- 📚 A fully searchable FAQ platform with dual-language support (English and Hindi)
- 🤖 **Yaksha** — an intelligent assistant driven by Gemini 2.0 Flash and enriched with the organization's internship knowledge resources.
- 👍 A **voting system** so interns can upvote/downvote FAQ helpfulness
- 📊 A live **server status** indicator and real-time clock
- 🌙 **Dark / Light mode** toggle with persistent preference

---
🏆 Impact

The portal streamlines information dissemination for internship participants by providing 24/7 access to verified resources, reducing dependency on manual support channels and improving the overall onboarding experience.
---
🤝 Acknowledgements

Developed during the Vicharanashala Internship Programme 2026 under the guidance of the team at IIT Ropar and supported by the Samagama Foundation.
---

## 🖥️ Tech Stack

| Layer | Technology |
|---------|---------|
| **Frontend** | React 19 + Vite 8 + React Router v7 |
| **Backend** | Python 3 + FastAPI + Uvicorn |
| **AI / Chat** | Google Gemini 2.0 Flash (`google-genai`) |
| **Styling** | Vanilla CSS |
| **Deployment** | Vercel + Render |
| **Data Storage** | JSON Flat Files |

---

## 🗂️ Project Structure

```text
IIT-Ropar/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Chatbot.jsx
│   │   │   ├── Header.jsx
│   │   │   ├── FAQItem.jsx
│   │   │   ├── ServerStatus.jsx
│   │   │   └── VoiceAssistant.jsx
│   │   ├── pages/
│   │   │   ├── Overview.jsx
│   │   │   └── FAQPage.jsx
│   │   ├── App.jsx
│   │   └── index.css
│   ├── .env
│   ├── .env.production
│   └── vercel.json
│
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   ├── faqs.json
│   ├── faqs_hi.json
│   ├── votes.json
│   └── .env
│
└── README.md
```

---

## ✨ Features

### 🔍 Searchable FAQ
- Instant search across all FAQs
- English ↔ Hindi language switch
- Category filtering
- Expand / Collapse controls

### 🤖 Yaksha AI Assistant
- Powered by Gemini 2.0 Flash
- Context-aware responses
- Internship knowledge-base integration
- Suggested questions
- Conversation history support

### 👍 Voting System
- Upvote / Downvote FAQ responses
- Optimistic UI updates
- Persistent local storage
- Backend synchronization

### 🎨 Modern UI/UX
- Glassmorphism design
- Dark / Light theme
- Responsive layout
- Smooth animations
- Live backend status indicator

---

## 🚀 Running Locally

### Prerequisites

- Node.js 18+
- Python 3.10+
- Google AI Studio API Key

### ⚙️ Backend Setup

```bash
cd backend

python -m venv venv

# Windows
venv\Scripts\activate

# Linux/macOS
source venv/bin/activate

pip install -r requirements.txt

echo GEMINI_API_KEY=your_key_here > .env

uvicorn main:app --reload
```

Backend runs on:

```text
http://localhost:8000
```

### 🎨 Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

Frontend runs on:

```text
http://localhost:5173
```

---

## 🌐 Deployment

| Service | Purpose |
|----------|----------|
| Vercel | React Frontend Hosting |
| Render | FastAPI Backend Hosting |

### Render Environment Variables

```env
GEMINI_API_KEY=your_gemini_api_key
```

### Vercel Environment Variables

```env
VITE_API_BASE=https://vicharanashala-internship.onrender.com/api
```

### Production URLs

```text
Frontend:
https://iit-ropar-seven.vercel.app

Backend:
https://vicharanashala-internship.onrender.com
```

---

## 🔌 API Reference

| Method | Endpoint | Description |
|----------|----------|----------|
| GET | /api/health | Health check |
| GET | /api/faqs?lang=en | English FAQs |
| GET | /api/faqs?lang=hi | Hindi FAQs |
| GET | /api/votes | Fetch votes |
| POST | /api/vote | Submit vote |
| POST | /api/chat | Chat with Yaksha AI |

---

## 👨‍💻 Author

Built with ❤️ for the **Vicharanashala Internship Programme 2026**

**IIT Ropar**  
Lab of Prof. Sudarshan Iyengar  
https://samagama.in
