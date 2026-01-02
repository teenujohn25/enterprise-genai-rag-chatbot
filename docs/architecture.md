# Architecture Overview

This project implements a Retrieval Augmented Generation (RAG) architecture for enterprise customer support.

## System Flow
1. Support content is ingested and split into chunks
2. Chunks are converted into vector embeddings
3. Vectors are stored in a FAISS index
4. User queries are embedded and matched against stored vectors
5. Retrieved context is used to generate grounded responses

## Design Decisions
- Backend-first architecture
- Hallucination prevention through retrieval grounding
- Notebook-based validation for rapid iteration
- API layer separated for deployment readiness

## Deployment Readiness
The system is designed to be deployed using OpenAI or Azure OpenAI models with minimal changes to the pipeline.
