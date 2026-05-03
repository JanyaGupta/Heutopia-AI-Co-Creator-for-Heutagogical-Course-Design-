# Heutopia-AI-Co-Creator-for-Heutagogical-Course-Design-

# Heutopia: AI Co-Creator for Heutagogical Course Design

## 🚀 Overview

**Heutopia** is an AI-powered learning platform that supports **self-determined (heutagogical) learning**. It helps students design their own learning paths, generate assessments, reflect on progress, and engage with adaptive educational tools using **AI (LLMs)**.

This project integrates **Django (backend)** with **local AI models (Ollama + Llama 3.1)** to create a personalized, interactive learning experience.

---

## 🎯 Key Features

### 🧠 AI-Powered Learning Path Generation

* Generates personalized learning plans based on:

  * Topic
  * Skill level
  * Learning goals
  * Preferred learning style
* Uses LLMs (Llama 3.1 via Ollama)

---

### 📝 Adaptive Assessments

* Automatically generates:

  * MCQs
  * True/False
  * Fill-in-the-blanks
  * Short answer questions
* Evaluates student responses and gives feedback

---

### 📊 Reflection & Feedback System

* Students submit reflections:

  * What they learned
  * Challenges faced
  * Confidence level
* AI generates constructive feedback

---

### ⚡ Active Learning Tools

* One Minute Paper (quick understanding checks)
* Story Mapping + AI feedback
* Muddiest Point clarification (AI explanations)

---

### 📚 Resource Recommendation

* AI suggests learning resources based on topic and level

---

### 📈 Progress Tracking

* Tracks completed topics
* Displays student progress visually

---

### 🎥 Media Library

* Provides curated:

  * Educational videos
  * Audio content

---

## 🏗️ Tech Stack

### Backend

* Python
* Django

### AI Integration

* Ollama
* Llama 3.1 (local LLM)
* LangChain (optional usage)

### Frontend

* HTML
* CSS
* Django Templates

### Database

* SQLite (development)

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/JanyaGupta/Heutopia-AI-Co-Creator-for-Heutagogical-Course-Design-.git
cd ai_heutagogy
```

---

### 2. Create Virtual Environment

```bash
python -m venv venv
```

Activate:

```bash
venv\Scripts\activate
```

---

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4. Install and Run Ollama

Download from:
https://ollama.com

Run:

```bash
ollama pull llama3.1
ollama run llama3.1
```

---

### 5. Run Django Server

```bash
python manage.py migrate
python manage.py runserver
```

---

### 6. Access the App

```
http://127.0.0.1:8000/accounts/login/
```

---

## 🔐 Authentication

* Uses Django’s built-in authentication system
* Login URL:

```
/accounts/login/
```

---

## 📂 Project Structure

```
ai_heutagogy/
│
├── core/                # Main Django project
├── student/             # Student app (learning features)
├── teacher/             # Teacher features
├── rag/                 # AI generation logic
├── templates/           # HTML templates
├── static/              # Static files
├── db.sqlite3           # Database
└── manage.py
```

---

## 🧠 AI Workflow

```
User Input → Django View → AI Generator (rag/) → Ollama → LLM Response → UI Display
```

---

## ⚠️ Limitations

* Requires local machine to run Llama 3.1
* Performance depends on:

  * RAM
  * CPU
* Not suitable for serverless deployment (e.g., Vercel)

---

## 🚀 Future Improvements

* Deploy using cloud LLM APIs (Groq/OpenAI)
* Add real-time streaming responses
* Enhance UI/UX
* Add collaborative learning features
* Optimize prompt engineering

---

## 🌐 Deployment Notes

* Django can be deployed on platforms like Render
* Ollama must be replaced with cloud APIs for production

---

## 👩‍💻 Author

**Janya Gupta**

---

## 📜 License

This project is for educational purposes.

---

## 💡 Acknowledgements

* Django
* Ollama
* Llama 3.1
* LangChain
