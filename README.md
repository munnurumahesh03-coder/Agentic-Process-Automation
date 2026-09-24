# 🤖 Agentic Process Automation (Cognitive Web Orchestrator)

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg )
![Playwright](https://img.shields.io/badge/Playwright-Automation-green.svg )
![CrewAI](https://img.shields.io/badge/CrewAI-Multi--Agent-orange.svg )
![Groq](https://img.shields.io/badge/Groq-Llama--3-black.svg )

## 📌 Enterprise Overview
Traditional Robotic Process Automation (RPA) relies on rigid, rule-based scripts (like XPath or Regex) that break the moment a website's UI changes. This project solves that problem by introducing **Cognitive UI Automation**. 

By orchestrating a multi-agent system using **CrewAI** and **Playwright**, this system autonomously navigates legacy web portals, dynamically parses complex DOM structures, and uses Large Language Models (LLMs) to transform messy, unstructured HTML into clean, validated JSON schemas without human intervention.

## 🚀 Core Features
*   **Multi-Agent Orchestration:** Utilizes CrewAI to divide tasks (Navigation, Data Extraction, and Structuring) among specialized AI agents.
*   **Self-Healing Navigation:** Playwright scripts integrated with AI fallbacks to bypass dynamic UI constraints and hidden folders.
*   **Cognitive Data Transformation:** Replaces brittle Regex with Groq's Llama-3 API to perform semantic extraction on unstructured text.
*   **Smart Deduplication & Merging:** Python-based logic groups scattered data across multiple web pages and merges them using unique identifiers.
*   **Production-Ready Output:** Converts raw portal data into analytics-ready JSON payloads.

## 🧠 System Architecture Workflow
1.  **Authentication Phase:** Securely navigates to the target portal and handles session logins.
2.  **Discovery Phase:** Expands all sidebar menus and maps the portal's complete DOM structure to harvest target URLs.
3.  **Agentic Routing:** Evaluates URLs against the target schema and dynamically routes the web spider only to pages containing relevant data.
4.  **Cognitive Parsing:** Extracts raw page text and passes it to the LLM for intent classification and entity extraction.
5.  **Load Phase:** Consolidates partial data into a master database and exports the final JSON schema.

## 🛠️ Tech Stack
*   **Core Logic:** Python
*   **Web Automation:** Playwright (Async/Sync DOM manipulation)
*   **AI Framework:** CrewAI, LangChain 
*   **LLM Provider:** Groq (Llama-3 70B/8B)
*   **Data Handling:** Pandas, JSON

## ⚙️ Installation & Setup
```bash
# Clone the repository
git clone https://github.com/your-username/Agentic-Process-Automation.git
cd Agentic-Process-Automation

# Install required dependencies
pip install -r requirements.txt

# Install Playwright browsers
playwright install chromium
