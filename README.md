# RAG Learn

A learning project exploring Retrieval-Augmented Generation (RAG) systems with LangChain, vector databases, and LLMs.

## Overview

This project demonstrates the core concepts of RAG pipelines:
- **Data Ingestion**: Load and process documents (text files, PDFs)
- **Embeddings**: Convert text to vector representations using sentence transformers
- **Vector Storage**: Store embeddings in vector databases (ChromaDB, FAISS)
- **Retrieval**: Find relevant documents based on semantic similarity
- **Generation**: Use LLMs (OpenAI, Groq) to generate responses based on retrieved context

## Project Structure

```
rag-learn/
├── main.py                 # Main entry point
├── pyproject.toml          # Project configuration and dependencies
├── requirements.txt        # Python dependencies
├── README.md               # This file
└── data-ingestion/
    ├── dataIngestion.ipynb # Notebook for data processing and experimentation
    └── data/
        └── text_files/    # Sample text documents
            ├── sample1.txt
            └── sample2.txt
```

## Requirements

- Python >= 3.13
- Virtual environment (venv, conda, etc.)

## Setup

### 1. Clone and Navigate to Project
```bash
cd rag-learn
```

### 2. Create Virtual Environment
```bash
python -m venv .venv
# On Windows
.venv\Scripts\activate
# On macOS/Linux
source .venv/bin/activate
```

### 3. Install Dependencies
```bash
uv pip install -r requirements.txt
# OR
pip install -r requirements.txt
```

## Dependencies

Core libraries:
- **langchain**: Framework for building LLM applications
- **langchain-openai**: OpenAI integration
- **langchain-groq**: Groq API integration
- **langchain-text-splitters**: Text chunking utilities
- **sentence-transformers**: Embeddings generation
- **chromadb**: Vector database
- **faiss-cpu**: Facebook AI Similarity Search
- **pypdf**: PDF parsing
- **pandas**: Data manipulation
- **python-dotenv**: Environment variable management
- **tiktoken**: Token counting for OpenAI models

## Configuration

Create a `.env` file in the project root for API keys:
```
OPENAI_API_KEY=your_key_here
GROQ_API_KEY=your_key_here
```

## Usage

### Run Main Script
```bash
python main.py
```

### Experimentation Notebook
Explore RAG concepts interactively:
```bash
jupyter notebook data-ingestion/dataIngestion.ipynb
```

## Next Steps

- [ ] Implement document loading and parsing
- [ ] Set up vector embeddings pipeline
- [ ] Configure vector database storage
- [ ] Build retrieval system
- [ ] Integrate LLM for response generation
- [ ] Add evaluation metrics

## Resources

- [LangChain Documentation](https://python.langchain.com/)
- [RAG Overview](https://python.langchain.com/docs/use_cases/question_answering/)
- [Sentence Transformers](https://www.sbert.net/)
- [ChromaDB](https://www.trychroma.com/)
