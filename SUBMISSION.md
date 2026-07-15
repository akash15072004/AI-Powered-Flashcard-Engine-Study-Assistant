
# 🎓 AI-Powered Flashcard Engine – Study Assistant

**Submitted by:** Akash Chaudhary
**Problem Chosen:** Study Assistant

---

# 🔗 Live Deployment

🚀 **Frontend (Vercel)**
👉 https://ai-powered-flashcard-engine-study-a-seven.vercel.app

⚙️ **Backend API (Render)**
👉 https://ai-powered-flashcard-engine-study.onrender.com

📘 **API Docs (Swagger)**
👉 https://ai-powered-flashcard-engine-study.onrender.com/docs

---

# 🎯 What I Built

I built an **AI-Powered Study Assistant** that converts PDF study materials into interactive flashcards using Large Language Models (LLMs). Instead of spending hours manually preparing notes and flashcards, students can simply upload a PDF, and the application automatically extracts the content and generates meaningful question-answer flashcards.

Unlike traditional flashcard applications, this system encourages **active recall** by allowing users to type their own answer before revealing the AI-generated answer. Users can then mark whether they answered correctly or incorrectly. Incorrect flashcards are automatically collected into a separate revision session, helping students focus on weak concepts instead of repeatedly reviewing everything.

The application is built as a complete full-stack solution with a React frontend, FastAPI backend, SQLite database, and Groq LLM integration.

---

# 🚀 Core Features

## 📄 1. PDF Upload & Intelligent Content Extraction

Students can upload lecture notes, textbooks, or study material in PDF format.

The backend:

* validates the uploaded file
* extracts readable text from the PDF
* cleans unnecessary formatting
* prepares structured content for AI processing

This removes the need to manually copy notes into the application.

---

## 🤖 2. AI Flashcard Generation

The extracted content is sent to the Groq LLM using carefully designed prompts.

The AI automatically identifies:

* important concepts
* definitions
* key facts
* technical terms
* explanations

and converts them into meaningful flashcards.

Each flashcard contains:

* Question
* Answer

instead of simply summarizing the text.

---

## 🧠 3. Active Recall Learning

Instead of immediately revealing the answer,

the learner first types their own answer.

After submission,

the correct AI-generated answer can be revealed.

This encourages:

* self testing
* better memory retention
* deeper understanding

rather than passive reading.

---

## ✅ 4. Self Evaluation

After viewing the answer,

users mark whether they answered correctly or incorrectly.

This creates a personalized learning experience.

---

## 🔁 5. Practice Incorrect Flashcards

One of the key features is targeted revision.

Instead of restarting the entire deck,

users can practice only the flashcards they previously answered incorrectly.

This helps learners spend more time on weak areas.

---

## 📈 6. Progress Tracking

The application keeps track of:

* Total Flashcards
* Correct Answers
* Incorrect Answers
* Remaining Cards
* Learning Progress

Students can continuously monitor their performance throughout the session.

---

## 🎨 7. Modern User Experience

The application provides

* Responsive Design
* Clean Interface
* Fast Navigation
* Mobile Friendly Layout
* Smooth Flashcard Navigation

making studying comfortable across devices.

---

# 🏗 System Architecture

### Frontend

* React.js
* Vite
* Tailwind CSS
* Axios

Responsible for

* Authentication
* PDF Upload
* Flashcard Interface
* Progress Display
* API Communication

---

### Backend

* FastAPI
* Python
* SQLAlchemy

Responsible for

* File Upload
* PDF Processing
* AI Integration
* Flashcard Generation
* Database Operations
* REST APIs

---

### Database

SQLite stores

* Users
* Flashcards
* Learning Sessions
* Progress Data

---

### AI Layer

Groq API

Model:

Llama 3

Used for

* Flashcard Generation
* Question Generation
* Concept Identification

---

### Deployment

Frontend

* Vercel

Backend

* Render

---

# 💡 Key Design Decisions

## Why PDF Upload?

Most students already have notes in PDF format.

Allowing direct uploads removes friction and makes the application practical.

---

## Why Active Recall?

Research consistently shows that recalling information from memory leads to stronger long-term retention than simply rereading notes. Active recall is a well-established learning technique used in many successful study tools. ([Quizgecko][1])

---

## Why Practice Incorrect Cards?

Instead of reviewing every flashcard repeatedly,

students focus only on concepts they struggle with,

making revision more efficient.

---

## Why FastAPI?

FastAPI provides

* High Performance
* Automatic API Documentation
* Easy AI Integration
* Asynchronous Support

making it ideal for AI applications.

---

# ⚙️ Challenges Faced

## Challenge 1

Generating useful flashcards from large PDFs.

### Solution

Implemented PDF preprocessing before sending content to the LLM.

This improved response quality significantly.

---

## Challenge 2

Frontend couldn't communicate with backend after deployment.

### Solution

Configured

* CORS
* Environment Variables
* Production API URLs

using Render and Vercel.

---

## Challenge 3

Handling AI response consistency.

### Solution

Designed better prompts that instruct the model to generate structured question-answer flashcards instead of generic summaries.

---

## Challenge 4

Keeping UI responsive during AI generation.

### Solution

Added loading indicators and asynchronous API requests to improve the user experience.

---

# 🔒 Security

Implemented

* Environment Variables
* CORS Protection
* Input Validation
* Secure REST APIs
* Backend-only API Keys

No AI keys are exposed to the frontend.

---

# 📊 Project Impact

The application helps students

* reduce manual note preparation
* revise faster
* remember concepts through active recall
* focus on weak topics
* improve revision efficiency

---

# 🔮 Future Improvements

Future versions will include

* AI-generated quizzes
* Spaced Repetition Scheduling
* Personalized Study Plans
* OCR for scanned PDFs
* Multi-language Flashcards
* Voice-based Study Mode
* AI Performance Analytics

---

# 📚 What I Learned

This project helped me gain hands-on experience in

* Full Stack Development
* React.js
* FastAPI
* REST API Development
* AI Integration
* Prompt Engineering
* Database Design
* Deployment using Render & Vercel
* Debugging Production Issues
* Environment Variable Management
* Frontend–Backend Communication

---





