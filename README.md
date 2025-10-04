# ZEGE — Web-Based IDE with AI Coding Assistant

## Overview
**ZEGE** is a full-stack web-based IDE that allows users to write, run, and debug code directly from the browser.  
It supports multiple programming languages and integrates AI code assistants — **ChatGPT**, **Gemini**, and **Blackbox** — for generating, explaining, and improving code in real time.

Designed for developers, students, and learners, ZEGE provides a seamless, intelligent coding environment for learning, experimenting, and rapid prototyping.

---

## Core Features

### Code Editor
- Monaco Editor with syntax highlighting  
- Language selection (Python, JavaScript, C++, Java, etc.)  
- Optional file management and tabbed editing  

### Code Execution
- Secure backend execution using Docker containers  
- Real-time output with stdout and stderr  
- Error tracking and runtime diagnostics  

### AI Integration
- Integrated ChatGPT, Gemini, and Blackbox assistants  
- Code generation, debugging, and explanation features  
- Side-by-side AI response comparison  

### Output Console
- Displays execution results in real time  
- Auto-scroll and clear console functionality  

### Optional Enhancements
- Light/Dark mode toggle  
- User authentication (Firebase or Auth0)  
- Save and share code snippets (MongoDB or Firestore)

---

## Tech Stack

**Frontend**
- React.js (Vite)
- Monaco Editor
- Tailwind CSS or ShadCN UI

**Backend**
- Node.js with Express  
- Docker (for sandboxed code execution)  
- WebSocket / REST API for real-time communication  

**AI Integration**
- OpenAI API (ChatGPT)  
- Gemini API  
- Blackbox AI API  

**Database (Optional)**
- MongoDB Atlas or Firebase Firestore  

---

## Project Structure

ZEGE/
├── frontend/ # React-based UI
│ ├── src/
│ │ ├── components/ # Editor, Console, AI Assistant
│ │ ├── pages/ # Home, Settings, Auth
│ │ └── App.jsx
│ └── package.json
│
├── backend/ # Express server
│ ├── routes/ # Code execution & AI routes
│ ├── controllers/ # Logic for AI & Docker handling
│ ├── docker/ # Sandbox scripts
│ └── server.js
│
└── README.md

yaml
Copy code

---

## Setup & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/ZEGE_CODE.git
cd ZEGE_CODE
2. Install Dependencies
bash
Copy code
# Frontend
cd frontend
npm install

# Backend
cd ../backend
npm install
3. Run the Application
bash
Copy code
# Start Backend
cd backend
npm run dev

# Start Frontend
cd ../frontend
npm run dev
4. Environment Configuration
Create .env files in both frontend/ and backend/ folders:

ini
Copy code
OPENAI_API_KEY=your_openai_key
GEMINI_API_KEY=your_gemini_key
BLACKBOX_API_KEY=your_blackbox_key
Future Enhancements
Multi-file project management

Live collaboration and pair programming

AI-powered code refactoring

Terminal input support

Built-in Git integration

Contributing
Contributions, feedback, and feature requests are welcome.
Please open a pull request or issue on the GitHub repository.
