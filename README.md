<div align="center">

# 🎬 AatoZen.AI-2


### **Where AI Meets Effortless Editing**

<p>
  <strong>AI-Orchestrated Video Editing • AI-Generated BGM • Modern Glass UI</strong>
</p>

<p>
  A production-ready monorepo for intelligent video editing and AI-powered background music generation.
</p>

<p>
  <img src="https://img.shields.io/badge/AI-Video%20Editing-8A2BE2?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Next.js-Frontend-000000?style=for-the-badge&logo=next.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-AI-4285F4?style=for-the-badge&logo=google&logoColor=white"/>
  <img src="https://img.shields.io/badge/Stability%20AI-BGM-FF6F61?style=for-the-badge"/>
</p>

<p>
  <a href="#-features">Features</a> •
  <a href="#-architecture">Architecture</a> •
  <a href="#-project-structure">Structure</a> •
  <a href="#-setup">Setup</a> •
  <a href="#-deployment">Deployment</a>
</p>

</div>

---

## ✨ What is AatoZen.AI?

**AatoZen.AI** is a production-ready AI video editing platform designed to make complex video editing workflows feel effortless.

Instead of manually constructing video-processing commands, the platform uses **AI orchestration** to translate editing requirements into executable video-processing operations.

It combines:

* 🤖 **Gemini-powered AI orchestration**
* 🎞️ **FFmpeg-based video processing**
* 🎵 **Stability AI-powered background music generation**
* ⚡ **FastAPI backend services**
* 🌐 **Next.js frontend**
* 💎 **Glassmorphism-based premium UI**
* 🧬 **Animated AI molecule background**
* ☁️ **Cloud-ready deployment**

### The Core Idea

```text
                 ┌─────────────────────┐
                 │       USER          │
                 │  Upload / Request   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │     NEXT.JS UI      │
                 │  Premium Glass UI   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │    FASTAPI API      │
                 │ Backend Orchestration│
                 └──────────┬──────────┘
                            │
                 ┌──────────┴──────────┐
                 ▼                     ▼
        ┌─────────────────┐   ┌─────────────────┐
        │   GEMINI AI     │   │   STABILITY AI  │
        │ FFmpeg Commands  │   │   BGM Generation │
        └────────┬────────┘   └────────┬────────┘
                 │                     │
                 └──────────┬──────────┘
                            ▼
                 ┌─────────────────────┐
                 │       FFmpeg        │
                 │  Video Processing   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │      OUTPUT         │
                 │ Preview / Download  │
                 └─────────────────────┘
```

---

# 🚀 Features

## 🤖 AI Video Orchestration

AatoZen.AI uses **Gemini-powered orchestration** to generate FFmpeg commands based on the requested editing workflow.

Instead of manually constructing complex FFmpeg operations:

```text
User Requirement
       ↓
Gemini AI
       ↓
FFmpeg Command Generation
       ↓
Video Processing
       ↓
Processed Video
```

---

## 🎵 AI Background Music

Generate background music using **Stability AI-powered BGM synthesis**.

The workflow integrates music generation directly into the editing experience.

```text
Music Requirement
       ↓
Stability AI
       ↓
AI-Generated BGM
       ↓
Video Integration
       ↓
Final Output
```

---

## 💎 Premium User Interface

AatoZen.AI features a modern visual interface built around:

* Glassmorphism
* Animated AI molecule background
* Clean interaction flows
* Modern component architecture
* Responsive frontend experience

The interface is designed to make AI-powered video editing feel simple rather than technically complex.

---

## ⚡ Streamlined Editing Workflow

The complete user workflow is designed around four simple stages:

```text
       📤 Upload
          ↓
       🤖 Orchestrate
          ↓
       👁️ Preview
          ↓
       📥 Download
```

### Upload → Orchestrate → Preview → Download

The goal is to keep the editing process as straightforward as possible while AI handles the underlying orchestration.

---

# 🏗️ Architecture

AatoZen.AI follows a **frontend + API backend + AI services + media-processing** architecture.

```text
                         ┌──────────────────────┐
                         │        USER          │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │      NEXT.JS         │
                         │      FRONTEND        │
                         │                      │
                         │ • Glass UI           │
                         │ • AI Molecule        │
                         │ • API Client         │
                         └──────────┬───────────┘
                                    │
                                  REST
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │       FASTAPI        │
                         │       BACKEND        │
                         │                      │
                         │ • API Routes         │
                         │ • Configuration      │
                         │ • Security           │
                         │ • Services           │
                         │ • Utilities          │
                         └───────┬───────┬──────┘
                                 │       │
                    ┌────────────┘       └────────────┐
                    ▼                                 ▼
          ┌──────────────────┐              ┌──────────────────┐
          │    GEMINI AI     │              │   STABILITY AI   │
          │                  │              │                  │
          │ FFmpeg command   │              │ BGM synthesis    │
          │ generation       │              │                  │
          └─────────┬────────┘              └─────────┬────────┘
                    │                                 │
                    └────────────────┬────────────────┘
                                     ▼
                          ┌─────────────────────┐
                          │       FFmpeg        │
                          │ Video Processing    │
                          └──────────┬──────────┘
                                     ▼
                          ┌─────────────────────┐
                          │       OUTPUT        │
                          │ Processed Media     │
                          └─────────────────────┘
```

---

# 📁 Project Structure

```text
AatoZen.AI/
│
├── backend/                         # FastAPI Backend
│   │
│   ├── app/
│   │   ├── main.py                  # Entry point & Routes
│   │   │
│   │   ├── core/                    # Config & Security
│   │   │
│   │   ├── services/                # Video & Music Logic
│   │   │
│   │   └── utils/                   # FFmpeg & Metadata
│   │
│   ├── uploads/                     # Input storage
│   │
│   ├── outputs/                     # Processed results
│   │
│   ├── .env                          # Credentials / API Keys
│   │
│   ├── requirements.txt
│   │
│   └── Dockerfile
│
├── frontend/                        # Next.js Frontend
│   │
│   ├── src/
│   │   ├── app/
│   │   │
│   │   ├── components/              # AI-molecule Background, Glass UI
│   │   │
│   │   └── lib/                     # API Client
│   │
│   ├── public/
│   │
│   ├── package.json
│   ├── next.config.js
│   └── tailwind.config.ts
│
└── README.md
```

---

# 🧰 Technology Stack

| Layer                  | Technology       |
| ---------------------- | ---------------- |
| 🎨 Frontend            | **Next.js**      |
| 🟦 Frontend Language   | **TypeScript**   |
| 🎨 Styling             | **Tailwind CSS** |
| ⚙️ Backend             | **FastAPI**      |
| 🐍 Backend Language    | **Python**       |
| 🧠 Video AI            | **Gemini**       |
| 🎵 Music AI            | **Stability AI** |
| 🎞️ Media Processing   | **FFmpeg**       |
| 🐳 Containerization    | **Docker**       |
| ☁️ Frontend Deployment | **Vercel**       |
| ☁️ Backend Deployment  | **Render**       |

---

# 🔄 End-to-End Workflow

```text
┌─────────────────────┐
│   1. Upload Video   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  2. Define Editing  │
│      Requirement    │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│   3. Gemini AI      │
│ Orchestrates Editing│
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  4. FFmpeg Command  │
│      Generation     │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  5. Video Processing│
└──────────┬──────────┘
           │
           ├──────────────────┐
           │                  │
           ▼                  ▼
┌──────────────────┐  ┌──────────────────┐
│ Stability AI BGM │  │ Processed Video  │
│    Generation    │  │                  │
└────────┬─────────┘  └────────┬─────────┘
         │                     │
         └──────────┬──────────┘
                    ▼
          ┌─────────────────────┐
          │       Preview       │
          └──────────┬──────────┘
                     │
                     ▼
          ┌─────────────────────┐
          │      Download       │
          └─────────────────────┘
```

---

# ⚙️ Setup

## 📋 Prerequisites

Make sure you have the required development environment available before starting the project.

* Python
* Node.js / npm
* FFmpeg
* Gemini API Key
* Stability AI API Key

---

## 🐍 Backend — FastAPI

### 1. Navigate to the backend

```bash
cd backend
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure API Keys

Create or update your `.env` file:

```env
GEMINI_API_KEY=your_gemini_api_key
STABILITY_API_KEY=your_stability_api_key
```

### 4. Start the backend

```bash
uvicorn app.main:app --reload
```

The FastAPI development server will start with hot reload enabled.

---

# 🌐 Frontend — Next.js

### 1. Navigate to the frontend

```bash
cd frontend
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the development server

```bash
npm run dev
```

### 4. Open the application

Visit:

**http://localhost:3000**

---

# 🔐 Environment Variables

AatoZen.AI requires API credentials for its AI-powered functionality.

```env
GEMINI_API_KEY=your_gemini_api_key
STABILITY_API_KEY=your_stability_api_key
```

### ⚠️ Security

Never commit real API keys to GitHub.

Keep credentials inside your `.env` configuration and ensure the file is excluded from version control.

---

# 🐳 Docker

The backend includes a `Dockerfile`, providing a containerization path for the FastAPI service.

```text
backend/
├── Dockerfile
├── requirements.txt
└── app/
```

This can be used as part of a production deployment workflow.

---

# ☁️ Deployment

## Production Deployment

AatoZen.AI is prepared for deployment using:

```text
             ┌────────────────────┐
             │     AatoZen.AI     │
             └─────────┬──────────┘
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
      ┌──────────────┐    ┌──────────────┐
      │    Vercel    │    │    Render    │
      │   Frontend   │    │   Backend    │
      └──────────────┘    └──────────────┘
             │                   │
             └─────────┬─────────┘
                       ▼
                  Live System
```

### Deployment Guide

A comprehensive deployment guide is available in the repository:

**[📘 Deployment Guide — DEPLOYMENT.md](https://github.com/chandramouli9392/AatoZen.AIPhase2/blob/main/DEPLOYMENT.md)**

The guide covers deploying:

* **Frontend → Vercel**
* **Backend → Render**

---

# 🎯 Design Philosophy

AatoZen.AI is built around a simple principle:

> **Complex editing should feel effortless.**

Instead of exposing users to complicated media-processing commands, the system places an AI orchestration layer between the user's intent and the underlying video-processing infrastructure.

```text
Traditional Editing

User
 ↓
Complex Tools
 ↓
Manual Configuration
 ↓
Commands
 ↓
Video Output


AatoZen.AI

User Intent
 ↓
AI Orchestration
 ↓
Automated Processing
 ↓
Preview
 ↓
Download
```

---

# 🧩 Core Components

### 🧠 Gemini AI

Responsible for AI-powered **FFmpeg command generation and video-editing orchestration**.

### 🎵 Stability AI

Responsible for **AI background music synthesis**.

### ⚙️ FastAPI

Provides the backend API layer responsible for connecting the frontend with video and music processing services.

### 🎨 Next.js

Provides the frontend experience and application interface.

### 🎞️ FFmpeg

Handles the underlying media-processing operations.

---

# 📊 Project Snapshot

| Category               | Details                                        |
| ---------------------- | ---------------------------------------------- |
| Project                | **AatoZen.AI**                                 |
| Purpose                | AI-orchestrated video editing & BGM generation |
| Architecture           | Production-ready monorepo                      |
| Frontend               | Next.js                                        |
| Backend                | FastAPI                                        |
| AI Video Orchestration | Gemini                                         |
| AI Music Generation    | Stability AI                                   |
| Video Processing       | FFmpeg                                         |
| UI                     | Glassmorphism + Animated AI Molecule           |
| Frontend Deployment    | Vercel                                         |
| Backend Deployment     | Render                                         |
| Containerization       | Docker                                         |

---

# 🛣️ Workflow at a Glance

```text
                  AATOZEN.AI
                      │
                      ▼
              ┌───────────────┐
              │     UPLOAD    │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │  ORCHESTRATE  │
              │    GEMINI     │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │    PROCESS    │
              │    FFMPEG     │
              └───────┬───────┘
                      │
             ┌────────┴────────┐
             ▼                 ▼
      ┌─────────────┐   ┌─────────────┐
      │  VIDEO      │   │     BGM     │
      │ PROCESSING  │   │ STABILITY AI│
      └──────┬──────┘   └──────┬──────┘
             │                 │
             └────────┬────────┘
                      ▼
              ┌───────────────┐
              │    PREVIEW    │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │    DOWNLOAD   │
              └───────────────┘
```

---

# 📦 Repository Resources

### 📖 README

**[Read the README](https://github.com/chandramouli9392/AatoZen.AIPhase2#readme-ov-file)**

### 🚀 Activity

**[View Repository Activity](https://github.com/chandramouli9392/AatoZen.AIPhase2/activity)**

### ⭐ Stars

**1 Star**

### 👀 Watchers

**0 Watchers**

### 🍴 Forks

**0 Forks**

### 📦 Releases

No releases published.

### 📦 Packages

No packages published.

---

# 👨‍💻 Contributor

<div align="center">

### **Chandramouli Boppana**

**[@chandramouli9392](https://github.com/chandramouli9392)**

Building AI-powered applications across:

`Generative AI` • `Machine Learning` • `Computer Vision` • `Backend Engineering`

</div>

---

# 💻 Repository Language Distribution

| Language   |     Usage |
| ---------- | --------: |
| TypeScript | **68.8%** |
| Python     | **27.9%** |
| CSS        |  **2.5%** |
| JavaScript |  **0.8%** |

---

# 🌟 Project Vision

AatoZen.AI brings together **generative AI, media processing, and modern web engineering** to create a simpler video-editing experience.

```text
        USER INTENT
             │
             ▼
       ┌─────────────┐
       │   AI        │
       │ ORCHESTRATOR│
       └──────┬──────┘
              │
       ┌──────┴──────┐
       ▼             ▼
    VIDEO           MUSIC
   EDITING         GENERATION
       │             │
       └──────┬──────┘
              ▼
          FINAL MEDIA
              │
              ▼
        PREVIEW → DOWNLOAD
```

### **AatoZen.AI**

> **Where AI Meets Effortless Editing.**

---

<div align="center">

## 🎬 Built with AI. Designed for Simplicity.

**© 2026 AatoZen.AI**

</div>
