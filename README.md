# LLMOps NSE RAG

A RAG-based LLMOps system that lets investors and traders query NSE (India) company quarterly financial results.

### Project Goal
Build a smart chatbot where users can ask questions like:
- "Compare TCS and Infosys revenue for last 5 years"
- "How has Reliance EPS trended in last 8 quarters?"

### Tech Stack (Phase 1)
- **LLM**: AWS Bedrock - Claude 3 Sonnet
- **Embeddings**: AWS Bedrock - Titan Text Embeddings v2
- **Vector DB**: Qdrant (local)
- **Frontend**: Streamlit
- **PDF Parsing**: pdfplumber + pandas
- **Language**: Python

### Current Phase
**Phase 1: Working MVP** (In Progress)

### Folder Structure
- `src/data_layer/` → PDF processing and chunking
- `src/embeddings/` → Bedrock embeddings
- `src/vector_db/` → Qdrant operations
- `src/rag/` → Retrieval + Generation logic
- `src/app/` → Streamlit UI
- `data/` → Sample PDFs and JSON files
- `notebooks/` → Experiments and testing

---
**Status**: Setting up project structure