# LangGraph Chatbot with Streamlit

A conversational AI chatbot built using:

- LangGraph
- LangChain
- Ollama (Llama 3)
- Streamlit
- SQLite Checkpointing
- Thread-based Chat Memory

## Features

✅ Interactive Streamlit Chat UI

✅ Conversation History

✅ Multiple Chat Threads

✅ Persistent Memory using SQLite

✅ Streaming AI Responses

✅ Local LLM (Llama 3 through Ollama)

✅ LangGraph Workflow

---

## Project Structure

```text
.
├── streamlit_frontend.py
├── streamlit_frontend_streaming.py
├── streamlit_frontend_threading.py
├── streamlit_frontend_database.py
│
├── langgraph_backend.py
├── langgraph_streaming_backend.py
├── langgraph_threading_backend.py
├── langgraph_database_backend.py
│
├── chatbot.db
├── requirements.txt
└── README.md
```

---

## Prerequisites

### Python

Recommended:

```bash
Python 3.12+
```

### Ollama

Install Ollama:

https://ollama.com/download

Pull Llama 3 model:

```bash
ollama pull llama3
```

Verify:

```bash
ollama list
```

---

## Installation

### Clone Repository

```bash
git clone <repository-url>
cd Langraph-Chatboat
```

### Create Virtual Environment

```bash
python -m venv myenv
```

Activate:

Mac/Linux:

```bash
source myenv/bin/activate
```

Windows:

```bash
myenv\Scripts\activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Ollama

Start Ollama:

```bash
ollama serve
```

Verify model:

```bash
ollama run llama3
```

---

## Run Applications

### Basic Chatbot

```bash
streamlit run streamlit_frontend.py
```

### Streaming Chatbot

```bash
streamlit run streamlit_frontend_streaming.py
```

### Thread-Based Chatbot

```bash
streamlit run streamlit_frontend_threading.py
```

### SQLite Database Chatbot

```bash
streamlit run streamlit_frontend_database.py
```

---

## LangGraph Memory

### In-Memory Checkpointer

```python
from langgraph.checkpoint.memory import InMemorySaver

checkpointer = InMemorySaver()
```

### SQLite Checkpointer

```python
from langgraph.checkpoint.sqlite import SqliteSaver

checkpointer = SqliteSaver.from_conn_string("chatbot.db")
```

---

## Technologies Used

- LangGraph
- LangChain
- Streamlit
- Ollama
- Llama 3
- SQLite
- Python

---

## Future Enhancements

- RAG with PDFs
- Vector Database Integration
- Agent Tools
- Web Search
- Multi-Agent Workflows
- Authentication

---

## Author

Vedvyas Kumar Rauniyar
