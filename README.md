# 🎓 Accelerated Development Plan: AI-Powered Feedback System via Canvas LTI

## 📘 Overview
This project develops a **functional prototype of an AI-driven feedback system** integrated into the **Canvas Learning Management System (LMS)** using the **Learning Tools Interoperability (LTI 1.3)** standard.

The system leverages **Large Language Models (LLMs)** (OpenAI GPT, Anthropic Claude, or Google Gemini) to provide:
- Automated evaluation of programming assignments  
- Multi-level, pedagogically aligned feedback  
- Personalized practice suggestions to address knowledge gaps  

The goal is to **enhance student learning and self-regulation** by delivering dynamic, context-aware, and scaffolded feedback within the familiar Canvas environment.

---

## 🧩 Objectives
- Integrate an **AI feedback engine** with Canvas using **LTI 1.3**  
- Generate **multi-level feedback** (Feedback Ladder) on programming submissions  
- Provide **personalized practice suggestions** based on detected learning gaps  
- Evaluate **usability, clarity, and pedagogical value** through informal user testing  

---

## 🧱 System Architecture
**Core Components:**

| Component | Description |
|------------|-------------|
| **Canvas LTI (1.3)** | Enables seamless LMS integration for assignment submissions and feedback display |
| **Python Backend** | Implements AI feedback logic, prompt engineering, and LTI communication |
| **LLM APIs** | Connects to OpenAI, Claude, or Gemini for natural language analysis and feedback generation |
| **PostgreSQL Database** | Stores course data, submissions, rubric metadata, and user interactions |
| **Streamlit** | Provides a rapid prototyping interface for AI feedback testing and instructor dashboarding |
| **Docker** | Containerizes the system for consistent deployment |

---

## ⚙️ Tech Stack
**Languages & Frameworks:**  
- Python 3.11  
- Streamlit (for rapid prototyping)

**Libraries:**  
- `openai`  
- `python-dotenv`  
- `requests`  
- `psycopg2`  

**Infrastructure:**  
- Docker  
- PostgreSQL  
- Git & GitHub for version control  

---

## 🚀 Development Phases

### Phase 1 – Foundation & LTI Exploration (Weeks 1–3)
- Set up Python environment, virtual environment, and dependencies  
- Conduct LTI 1.3 “Hello World” integration test in Canvas sandbox  
- Test API connectivity with selected LLMs  
- Compare OpenAI, Claude, and Gemini responses for feedback accuracy  

### Phase 2 – Core Feedback Engine V1 (Weeks 4–7)
- Implement assignment submission handling via LTI  
- Develop initial prompt templates for syntax, logic, and rubric-based feedback  
- Integrate linter outputs to augment LLM context  
- Display AI-generated feedback inside Canvas or via Streamlit prototype  

### Phase 3 – Enhanced Feedback & Practice Suggestions (Weeks 8–10)
- Implement multi-level “Feedback Ladder” (Levels 0–4)  
- Add personalized practice recommendations based on detected gaps  
- Refine prompts with chain-of-thought and few-shot techniques  

### Phase 4 – Integration, Testing & Refinement (Weeks 11–12)
- Perform end-to-end system integration within Canvas  
- Conduct qualitative user testing with students and instructors  
- Fix bugs, refine feedback presentation, and finalize documentation  

---

## 🧠 Feedback Ladder Structure

| Level | Type | Description |
|--------|------|-------------|
| 0 | Verdict | Indicates correctness or error presence |
| 1 | Error Location | Shows failing input/output or error line |
| 2 | Hint | Conceptual clue about the issue |
| 3 | Logical Focus | Narrows down likely mistake location |
| 4 | Edit Suggestion | Provides a concrete code fix proposal |

---

## 🔍 Evaluation Focus
- **Usability:** Clarity, latency, and user interaction within Canvas  
- **Pedagogical Value:** How feedback supports understanding and improvement  
- **Trust & Authenticity:** Student perceptions of AI-generated feedback  
- **Self-Regulated Learning (SRL):** Evidence of improved planning and reflection  

---

## 📈 Expected Deliverables
- Functional **Canvas-integrated AI feedback prototype**  
- Documentation of **LTI integration process** and constraints  
- **Feedback Ladder engine** with sample prompts and responses  
- **Practice suggestion module** linked to learning objectives  
- **Streamlit demo interface** for independent feedback testing  

---

## 🧪 Future Work
- Extend support for diverse assignment types (text, essays, design docs)  
- Enable instructor dashboards for monitoring AI feedback quality  
- Integrate knowledge-tracing models for adaptive personalization  
- Conduct controlled pedagogical studies on learning outcomes and SRL impact  
