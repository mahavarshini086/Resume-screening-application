

# 🤖 Agentic Resume Screening System

An **Agentic AI-powered Resume Screening System** that autonomously evaluates resumes against job descriptions using multiple intelligent agents.
The system mimics how a human recruiter reasons—by parsing resumes, extracting skills, scoring relevance, and generating explainable hiring insights.

Built to demonstrate **agent-based reasoning, orchestration, and evaluation**, this project aligns with modern **enterprise AI hiring workflows**.

---

## 🚀 Key Features

* 🧠 **Multi-Agent Architecture**

  * Resume Parser Agent
  * Job Description Analyzer Agent
  * Skill Matching & Scoring Agent
  * Decision & Explanation Agent

* 📄 Automated resume parsing (PDF/DOCX)

* 📊 Resume–JD relevance scoring

* 🧩 Skill gap analysis

* 📝 Explainable screening decisions

* ⚡ Handles multiple resumes in batch

* 🔒 Injection-safe prompt design (DEFEND-style hardening)

---

## 🏗️ System Architecture

```
User Input (Resumes + JD)
        ↓
Resume Parser Agent
        ↓
JD Analysis Agent
        ↓
Skill Matching Agent
        ↓
Decision Agent
        ↓
Final Ranking + Explanation
```

---

## 🛠️ Tech Stack

* **Python**
* **LLMs (Gemini / OpenAI / OpenRouter)**
* **LangChain / Agent Orchestration**
* **PyPDF / Docx**
* **Vector Embeddings (optional)**
* **Streamlit / FastAPI (UI / API layer)**

---

## 📁 Project Structure

```
agentic-resume-screening/
│
├── agents/
│   ├── resume_parser.py
│   ├── jd_analyzer.py
│   ├── skill_matcher.py
│   └── decision_agent.py
│
├── data/
│   ├── resumes/
│   └── job_description.txt
│
├── app.py
├── config.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup & Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/agentic-resume-screening.git
cd agentic-resume-screening
```

### 2️⃣ Create virtual environment

```bash
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Add API Key

Create a `.env` file:

```env
LLM_API_KEY=your_api_key_here
```

---

## ▶️ Run the Application

```bash
python app.py
```

or (if Streamlit UI is enabled):

```bash
streamlit run app.py
```

---

## 📊 Example Output

* Candidate Name
* Matching Score (0–100)
* Matched Skills
* Missing Skills
* Hiring Recommendation
* Natural-language Explanation

---

## 🔍 Why Agentic?

Unlike rule-based ATS systems, this project uses **autonomous agents** that:

* Reason independently
* Collaborate sequentially
* Validate outputs before decision making

This makes the system:

* More accurate
* More explainable
* More enterprise-ready

---

## 🔐 Prompt Security

* Context isolation
* Instruction hierarchy enforcement
* User input sanitization
* Output validation

Designed to resist **prompt injection and resume manipulation attacks**.

---



## 👨‍💻 Use Cases

* HR automation
* ATS augmentation
* Campus hiring
* Resume shortlisting platforms
* Enterprise AI demos

---

