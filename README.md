# Grounded Market Intelligence with Multi-Agent AI Pipeline
Market Intelligence AI Agents automate the creation of evidence-based business reports. Using sequential Gemini-powered agents and Google Search, the system fetches, analyzes, and summarizes real-time news to deliver actionable, trustworthy insights for decision-makers.

**Subtitle:**  
Automated, evidence-based business insights with Gemini-powered agents and real-time data
  
*(Replace with your actual card/thumbnail image, size 560x280)*

***

## Table of Contents

- [Problem Statement](#problem-statement)
- [Why Agents?](#why-agents)
- [Architecture](#architecture)
- [Demo](#demo)
- [How to Run](#how-to-run)
- [Technologies Used](#technologies-used)
- [Links & Resources](#links--resources)
- [Author](#author)

***

## Problem Statement

Business leaders and analysts face enormous challenges making timely decisions: traditional market research is slow, expensive, and often speculative. There’s a growing need for automated, reliable, and transparent market intelligence – insights drawn directly from real-world, reputable sources and delivered instantly.

***

## Why Agents?

Agents are the ideal solution for modular, explainable, and adaptive workflows:
- **Specialization:** Each agent handles a clear subtask—search, fetch, analyze, synthesize, and report.
- **Orchestration:** Agents pass output in order, ensuring clarity, traceability, and reliability.
- **Grounding:** By integrating tools like Google Search, agents deliver fact-based answers, eliminating AI speculation and hallucination.
- **Flexibility:** Easy to extend, modify, or parallelize the pipeline for new sources or tasks.

***

## Architecture

```
[Google Search Tool] → [Fetch Agent] → [Analysis Agent] → [Synthesis Agent] → [Report Agent] → [Final Report]
```

**Agents:**
1. **Google Search Agent**: Finds recent, relevant news articles.
2. **Fetch Agent**: Curates and formats articles.
3. **Analysis Agent**: Assesses sentiment, events, and trends.
4. **Synthesis Agent**: Summarizes actionable insights.
5. **Report Agent**: Compiles everything into a professional report.

*All agents orchestrated using `SequentialAgent` (ADK Python).*

***

## Demo

### Example Workflow

1. **Input:**  
   - User specifies a company and topic (e.g., "Tesla" and "battery technology").
2. **Output:**  
   - The agent pipeline fetches the latest news, analyzes sentiment & trends, summarizes core insights, and creates a market intelligence report.

### How to Run

#### Kaggle Notebook
- Open `final-project.ipynb` in Kaggle (or Jupyter).
- Replace `"GEMINI_API_KEY"` with your own API key:
    ```python
    import os
    os.environ["GEMINI_API_KEY"] = "your_api_key_here"
    ```
- Execute notebook cells in order.
- Enter your company/topic, and view the report output.

**No API keys/secrets included in repository—please supply your own in a secure `.env` or environment variable.**

***

## Technologies Used

- **Google Agent Development Kit (ADK)**
- **Gemini 2.5 Flash Lite (LLM)**
- **Python 3.11+**
- **Streamlit** (optional UI)
- **Gradio** (optional UI/demo)
- **Google Search Tool** (AgentTool integration)
- **Markdown, Diagrams, and Notebooks**

***

## Links & Resources

- [Kaggle Notebook]([YOUR_KAGGLE_NOTEBOOK_LINK](https://www.kaggle.com/code/nuclearforce123/final-project-multi-agent))
- [ADK Python Docs](https://google.github.io/adk-docs/)
- [Gemini](https://ai.google.dev)
- [Competition Page](https://www.kaggle.com/competitions/agents-intensive-capstone-project)

***

## Author

**Name:** SUBASH CHANDRA BOSE M.
**Contact:** subash.exec@gmail.com
