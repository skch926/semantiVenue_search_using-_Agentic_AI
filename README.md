# SemantiVenue AI

SemantiVenue-AI is an AI-powered research paper conference recommendation system using LangGraph.

## Setup

1. Install Ollama and pull model: `ollama pull llama3.2`
2. `pip install -r requirements.txt`
3. `python build_vector_db.py`
4. `streamlit run app/streamlit_app.py`




The project uses:
- Ollama for local LLM inference
- LangChain + LangGraph for AI workflow
- ChromaDB for vector search
- Streamlit for the frontend
- Sentence Transformers for embeddings

The system analyzes research papers and recommends the most suitable conferences.

---

# Features

- Research paper analysis
- Conference recommendation
- Semantic search using embeddings
- Vector database retrieval
- Reranking pipeline
- Local LLM support with Ollama
- Interactive Streamlit UI

---

# Tech Stack

## Backend
- Python
- LangChain
- LangGraph
- ChromaDB
- Ollama

## Frontend
- Streamlit


---

# Project Structure

```text
SemantiVenue-AI/
│
├── app/
│   └── streamlit_app.py
│
├── src/
│   ├── paper_processor.py
│   ├── retriever.py
│   ├── reranker.py
│   ├── evaluator.py
│   ├── graph.py
│   ├── pipeline.py
│   └── evaluation_metrics.py
│
├── data/
│   └── conferences.json
│
├── build_vector_db.py
├── requirements.txt
├── README.md
└── .env
