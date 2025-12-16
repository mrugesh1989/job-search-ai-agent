# 🚀 Job-Search-AI-Agent

An **agentic AI job search assistant** built with the **CrewAI framework** and powered by **Gemini LLM**.  
This project automates job discovery, salary analysis, company‑specific searches, and career guidance — all through intelligent agents and custom tools.

---

## ✨ Features
- **Agentic AI Architecture**
  - Multiple specialized agents (JobSearchAgent, CompanyTargetedAgent, EntryLevelAgent, AnalysisAgent, MessageWriterAgent)
  - Each agent has a defined role, goal, and backstory
- **Smart Job Search**
  - Quick search, salary‑focused search, company‑targeted search, entry‑level search, and full search
- **Career Guidance**
  - Provides skill gap analysis, career progression insights, and tailored recommendations
- **Automation Tools**
  - Integrated with SerpAPI for job listings
  - File and directory tools for saving and analyzing results
- **Interactive CLI**
  - Run searches via `run_search.py` with a simple menu
  - Setup preferences interactively with `setup_job_search.py`

---

## 🛠️ Tech Stack
- **Python 3.13+**
- **CrewAI** (Agent & Task orchestration)
- **Gemini LLM** (via API)
- **SerpAPI Google Jobs API**
- **dotenv** for environment configuration

---

## 📂 Project Structure

- agents.py          # Defines specialized agents
- tasks.py           # Task definitions for job search & analysis
- tools.py           # Custom tools for search, salary, company targeting
- config.py          # User job search preferences
- config_examples.py # Example configurations for different roles
- main.py            # Core orchestration logic
- run_search.py      # Interactive CLI for job search
- setup_job_search.py# Interactive setup for config

---

## ⚙️ Setup & Installation

1. **Clone the repository**

    ```bash
    git clone https://github.com/mrugesh1989/job-search-ai-agent.git
    cd src/

2. **Install Dependencies**

    ```bash 
    pip install -r requirements.txt

3. **Set environment variables**

    ```bash
    SERPER_API_KEY=your_serper_api_key
    GEMINI_API_KEY=your_gemini_api_key
    GEMINI_MODEL=gemini-2.5-flash

4. **Run Setup**

    ```bash
    python setup_job_search.py

5. **Start Job Search**

    ```bash
    python run_search.py
  

## 🖥️ Example Output

- **Quick Search**

Quick search results for 'Software Engineer remote' (5 jobs):

1. Software Engineer at Google
   📍 Remote | 💰 $150,000 | 📅 2 days ago
   🔗 https://careers.google.com/job/12345

- **Salary Focused Search**

Found 3 Software Engineer jobs with salary information:

1. **Backend Developer**
   Company: Microsoft
   Location: Remote
   Salary: $160,000
   Link: https://careers.microsoft.com/job/67890