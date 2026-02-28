# Project Context - LLMOps NSE RAG

## Project Summary
A RAG-based system where investors can query NSE Nifty 50 
company quarterly financial results using natural language.

## Current Phase
Phase 1 - Working MVP (In Progress)

## Tech Stack Decisions
- PDF Parsing: pdfplumber + pandas (reason: handles text + tables well)
- LLM: AWS Bedrock Claude 3 Sonnet (reason: strong reasoning for financial data)
- Embeddings: AWS Bedrock Titan Text Embeddings v2
- Vector DB: Qdrant local Docker (reason: rich metadata filtering)
- Frontend: Streamlit (reason: simple and fast for MVP)
- No LangChain/LlamaIndex (reason: learning raw implementation)

## Folder Structure
- src/data_layer/  → PDF processing and chunking
- src/embeddings/  → Bedrock Titan embeddings
- src/vector_db/   → Qdrant store and search
- src/rag/         → Retrieve chunks + Generate answer
- src/app/         → Streamlit UI
- data/            → Sample PDFs and processed JSON
- notebooks/       → Small experiments

## Progress Tracker
- [x] GitHub repo created
- [x] Folder structure created
- [x] README updated
- [x] project_context.md created
- [ ] AWS S3 bucket setup
- [ ] Bedrock access enabled
- [ ] PDF processor built
- [ ] Embeddings pipeline built
- [ ] Qdrant ingestion built
- [ ] RAG logic built
- [ ] Streamlit UI built

## Functions Built So Far
(keep updating this as we build)

## Doubts / Decisions Pending
(note down anything unclear here)