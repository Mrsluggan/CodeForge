# 🚀 CodeForge – Real-Time Collaborative Code Editor

**CodeForge** is a full-stack, real-time collaborative code editor inspired by the editing experience of Google Docs and the version control mindset of Git – built entirely in Java with a modern tech stack.

> “Collaborate. Code. Version. All in real-time.”

---

## 🎯 Features

- 🧠 **Multi-user Real-Time Editing** (WebSocket-based)
- ✨ **Syntax Highlighting** for Java, JavaScript, Python (Monaco Editor)
- 📂 **Project + File Management**
- 🔄 **Auto Versioning** – no need to hit save
- 🔐 **OAuth2 Authentication** (Google, GitHub)
- 📜 **Version History** with Diff View
- 👥 **Live Presence** – see who is editing
- 🧾 **Role-Based Access Control** (Owner, Editor, Viewer)
- 🐳 **Dockerized Deployment**

---

## 🛠️ Tech Stack

### Backend
- Java 17 + Spring Boot 3
- Spring WebSocket (STOMP over SockJS)
- Spring Security + OAuth2
- MongoDB (versioned document storage)
- Redis (real-time collaboration state)
- Docker + Docker Compose
- JUnit + Mockito + Testcontainers

### Frontend (optional)
- React + TypeScript
- Monaco Editor (used in VSCode)
- Tailwind CSS
- STOMP.js for WebSocket client

---

## 🧱 Architecture

CodeForge is built using a modular architecture:


Each component is stateless and horizontally scalable.

---

## 🔍 Core Challenges Solved

- ✅ WebSocket authentication with JWT tokens
- ✅ Optimized document syncing using CRDT-like delta storage
- ✅ Real-time conflict resolution for concurrent editing
- ✅ Efficient diff + version tracking in MongoDB
- ✅ Stateless WebSocket architecture with Redis pub/sub

---

## 📸 Screenshots (Optional)

*(Insert screenshots of the editor, real-time sync, diff viewer, etc.)*

---

## 🚀 Getting Started

```bash
# Clone repository
git clone https://github.com/yourusername/codeforge.git

# Start using Docker
docker-compose up --build
