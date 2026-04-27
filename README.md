# AI-Multi-Agent-System
A professional Multi-Agent Research System using LangGraph, Groq (Llama 3), and Tavily. Features a structured Planner-Researcher-Writer workflow with a Gradio UI.

## 📺 Project Demo
<!-- Video Link here -->

https://github.com/user-attachments/assets/8ac76fcd-9ef8-41fb-b030-96ccb5c67348

*A brief walkthrough of the Multi-Agent workflow and Gradio interface.*

# Multi-Agent AI Researcher & Writer

An advanced AI-powered multi-agent system built with **LangGraph**, **Groq (Llama 3.3)**, and **Tavily**. This application uses a collaborative agent workflow (Planner -> Researcher -> Writer -> Critic) to provide high-quality, researched answers via a sleek **Gradio** web interface.

## Key Features

- **Multi-Agent Orchestration**: Leverages **LangGraph** to manage complex states and transitions between specialized agents.
- **Hierarchical Workflow**: 
  - **Planner**: Deconstructs user queries into actionable, strategic steps.
  - **Researcher**: Executes real-time web searches using the **Tavily API**.
  - **Writer**: Synthesizes raw research into cohesive, professional, and cited responses.
  - **Critic**: Reviews final drafts for quality and factual accuracy before output.
- **High-Performance Inference**: Powered by **Groq (Llama-3.3-70b)** for near-instantaneous response times.
- **Stateful Memory**: Integrated `MemorySaver` to maintain seamless conversation context for follow-up queries.
- **Interactive Web UI**: A clean dashboard built with **Gradio** for an intuitive user experience.

## 🛠️ Tech Stack

- **Framework**: [LangChain](https://langchain.com) & [LangGraph](https://github.io)
- **LLM**: Groq (Llama-3.3-70b-versatile)
- **Search Engine**: [Tavily AI](https://tavily.com)
- **UI Layer**: [Gradio](https://gradio.app)
- **Language**: Python 3.10+

## Quick Start (Google Colab)

1. **Upload**: Open the `.ipynb` file in Google Colab.
2. **Setup Keys**: 
   - Go to **Secrets** (🔑 icon).
   - Add `GROQ_API_KEY` and `TAVILY_API_KEY`.
   - Toggle **"Notebook access"** to ON.
3. **Run**: Install dependencies and execute all cells to launch the interface.

## System Architecture

The graph follows a structured state-machine logic:
`START ➔ Planner ➔ Researcher ➔ Writer ➔ Critic ➔ END`

Each node communicates through a shared `MultiAgentState`, ensuring data integrity throughout the research process.

## 📄 License

This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for more details.



