# Investment Research Agent - Multi-Agent System
AAI-520 Final Project: Advanced AI Investment Research System

**University Of San Diego - AAI 520 - Natural Language Processing and GenAI**

**Final Team Project**: Multi-Agent Financial Analysis System

**Group**: 08

**Contributors**:
- Swapnil Patil (spatil@sandiego.edu)
- Christopher Akeibom Toh (cakeibomtoh@sandiego.edu)
- Nelson Arellano Parra (narellanoparra@sandiego.edu)

## Project Overview

This project implements a comprehensive Investment Research Agent using multiple AI agent patterns and Azure OpenAI. The system demonstrates advanced autonomous AI capabilities for investment analysis and decision-making.

## Requirements

### **Agent Functions (33.8%)**
- **Plans research steps** for given stock symbols using structured planning
- **Uses tools dynamically** with Yahoo Finance, NewsAPI, FRED, and Alpha Vantage APIs
- **Self-reflects** to assess output quality across multiple dimensions
- **Learns across runs** using FAISS vector database for persistent memory

### **Workflow Patterns (33.8%)**
1. **Prompt Chaining**: News Ingest → Preprocess → Classify → Extract → Summarize
2. **Routing**: Directs analysis to specialist agents (Technical, Fundamental, News)
3. **Evaluator-Optimizer**: Generate → Evaluate → Refine using Azure OpenAI

### **Technology Stack**
- **Python** with LangChain framework
- **Azure OpenAI API** for all LLM operations
- **Data Sources**: Yahoo Finance (yfinance), NewsAPI, FRED, Alpha Vantage
- **Vector Database**: FAISS for persistent agent memory
- **Visualization**: Matplotlib, Seaborn, Plotly for comprehensive charts
- **Web Interface**: Gradio for interactive analysis

## Deliverable Files

1. **`investment_research_agent.ipynb`** - Main notebook with complete system
2. **`.env`** - Environment configuration with API keys
3. **`README.md`** - This documentation file

## Quick Start

1. **Install Dependencies**:
```bash
pip install langchain langchain-openai langchain-community yfinance pandas numpy matplotlib seaborn plotly gradio faiss-cpu python-dotenv requests fredapi newsapi-python
```

2. **Configure Environment**: API keys are already configured in `.env`

3. **Run the Notebook**: Execute all cells in `investment_research_agent.ipynb`

4. **Use Interface**: The Gradio web interface will launch for interactive analysis

This implementation demonstrates state-of-the-art autonomous AI capabilities for investment research, fulfilling all project requirements while providing a professional-grade analysis system.
