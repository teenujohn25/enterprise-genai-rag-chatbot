# Enterprise Customer Support GenAI Chatbot (RAG)

This project implements an enterprise-style customer support chatbot using a Retrieval Augmented Generation (RAG) architecture. The system answers user queries strictly based on approved support documentation, preventing hallucinations.

## Problem Statement
Customer support teams frequently handle repetitive queries related to accounts, billing, and general usage. This project demonstrates how a GenAI system can automate first-level support while remaining grounded in company knowledge.

## Architecture Overview
The solution follows a standard RAG pipeline:
1. Support documents are ingested and chunked
2. Text chunks are converted into vector representations
3. Vectors are stored in a FAISS index for semantic retrieval
4. Relevant context is retrieved at query time
5. Responses are generated strictly from retrieved context

The architecture is designed to be deployable using OpenAI or Azure OpenAI models.

## Repository Structure
