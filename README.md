# noto – AI-Powered Learning Assistant

KnowBuddy is a full-stack web application designed to help students and independent learners understand and retain information more effectively. Users can upload documents or notes, ask AI-powered questions, generate quizzes and flashcards, and take structured notes — all within an integrated study environment.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Core Features](#core-features)
- [Tech Stack](#tech-stack)
- [Infrastructure and Management](#infrastructure-and-management)
- [Pages and Functionality](#pages-and-functionality)
- [Optional Enhancements](#optional-enhancements)
- [Setup Instructions](#setup-instructions)
- [Directory Structure](#directory-structure)
- [Planned Deployment](#planned-deployment)

---

## Project Overview

This project is a self-directed effort to build a feature-rich, AI-enhanced educational platform that showcases strong backend, frontend, cloud, and DevOps integration skills. It is designed to demonstrate proficiency with tools such as SQL, Express.js, React, Node.js, Docker, AWS, and Kubernetes while incorporating intelligent features powered by the OpenAI API.

---

## Core Features

1. **User Authentication**
   - Secure signup and login using JWT
   - Guest access mode with limited features
   - User onboarding tutorial on first login

2. **Ask Page (Document Q&A)**
   - Upload and parse documents (PDF, DOCX, TXT)
   - Ask contextual questions about the content using OpenAI
   - Summarize entire documents or selected sections
   - Request elaboration or breakdowns of complex topics
   - Store Q&A history for future reference

3. **Learn Page (AI Study Tools)**
   - Upload personal notes, slides, or curricula
   - Generate:
     - Flashcards (term-definition format)
     - Quizzes (multiple choice, true/false)
     - Summaries or study guides
   - Save, edit, and organize generated content into study decks

4. **Personal Notebook**
   - Floating note-taking interface accessible from all pages
   - Markdown support with auto-save
   - Diagram/sketch drawing using canvas or SVG
   - Tag-based organization of notes by topic
   - Export notes as PDF or Markdown

5. **Dashboard**
   - View activity statistics: flashcards reviewed, quizzes taken, questions asked
   - Recent uploads and documents
   - Personalized suggestions or reminders

6. **Study Deck Organizer**
   - Create and manage flashcard decks
   - Organize cards by subject, difficulty, or tags
   - Practice mode with shuffle/retry incorrect options
   - Revision scheduling (spaced repetition logic as optional enhancement)

---

## Tech Stack

**Frontend**
- React.js (Vite or Create React App)
- Context API or Redux for global state
- Axios for API calls

**Backend**
- Node.js with Express.js
- RESTful API
- JWT-based authentication and authorization

**Database**
- SQL (PostgreSQL or MySQL)
- Hosted on AWS RDS

**AI Integration**
- OpenAI API (GPT-4 or GPT-3.5)
- Document summarization, Q&A, flashcard, and quiz generation

---

## Infrastructure and Management

**AWS**
- RDS for SQL database
- S3 for file storage (uploaded documents, drawings)
- Optional: EC2 or EKS for hosting

**Docker**
- Containerization of frontend and backend
- Shared environment using `docker-compose.yml`

**Kubernetes**
- Microservice orchestration (optional; planned for deployment stage)
- Separate pods for backend API, frontend, and worker services

**CI/CD**
- GitHub Actions configured for:
  - Build and test pipeline
  - Docker image creation
  - Optional: Deploy to AWS (ECS/EKS)

**Testing**
- Jest for:
  - Backend unit tests (routes, services, OpenAI calls)
  - Frontend unit and integration tests (component rendering, state changes)

---

## Pages and Functionality

### Welcome Page
- Login and registration forms
- Guest access option
- Brief tutorial/walkthrough

### Ask Page
- Document upload and display
- Text parsing
- Chat-style Q&A interface with AI
- Summary and elaboration buttons
- Q&A log saved to user history

### Learn Page
- Upload notes or slides
- Choose generation type: flashcards, quizzes, summaries
- Editable output with save-to-deck feature

### Notebook (Popup)
- Always-available floating editor
- Note-taking with markdown support
- Drawing/sketching tool for visual learners
- Save notes by subject or session

### Dashboard
- Visual overview of progress
- History of activity (uploads, Q&A, flashcard practice)
- Suggestions for next steps or review

### Deck Organizer
- Tag-based deck creation
- Practice sessions
- Filter, edit, and delete cards
- Revision scheduling (stretch goal)

---

## Optional Enhancements

- AI-powered search across all user content
- Dark/light mode toggle

---
