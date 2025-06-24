# Simple AI Agent Using MCP Tools

This project is a terminal-based AI agent built using **LangGraph**, **OpenAI GPT-4o**, and **Firecrawl**, enabling dynamic web scraping and crawling via MCP tools.

The agent uses the **Model Context Protocol (MCP)** to connect to external tools over `stdio`, allowing flexible integration and tool orchestration in an interactive session.

---

## Features

- AI-powered conversational agent using `gpt-4o-mini`
- Step-by-step reasoning via LangGraph's `React Agent`
- Website crawling and scraping with [Firecrawl MCP Tool](https://github.com/firecrawl/firecrawl)
- Dynamic loading of tools via `langchain_mcp_adapters`
- Fully terminal-driven interaction

---

## Technologies Used

- [LangGraph](https://docs.langgraph.dev/)
- [LangChain MCP Adapters](https://github.com/langchain-ai/langchain/tree/master/libs/community/langchain-community/tools/mcp)
- [OpenAI GPT-4o](https://platform.openai.com/)
- [Firecrawl MCP](https://github.com/firecrawl/firecrawl)
- Python 3.10+
- AsyncIO, dotenv, MCP client

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/mcp-firecrawl-agent.git
cd mcp-firecrawl-agent

```

### 2. Set Up Python Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt

```

### 3. Install Node.js and Firecrawl

```bash
npm install -g firecrawl-mcp

```

### 4. Environment Variables

Set the environment variables

```bash
OPENAI_API_KEY= " "
FIRECRAWL_API_KEY= " "

```
---

## How It Works

Launches Firecrawl MCP server via npx firecrawl-mcp

Loads tools using MCP stdio protocol

Creates a LangGraph agent that can use tools automatically based on your queries

Lets you interact with the tools in real time through the terminal

---
## How It Works

run python main.py in the terminal

You will see the available tools, and then can type questions like:

```bash
You: Find articles on climate change from the past week.
You: Summarize the content of https://example.com

```

Type quit to exit the session

---

## File Structure

```bash
mcp-firecrawl-agent/
├── main.py              # Main agent code
├── .env                 # Environment variables
├── README.md            # This file
└── requirements.txt     # Python dependencies

```

---


## License

This project is open-source and available under the MIT License

---

## Acknowledgement

Tech with Tim
