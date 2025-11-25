# 🚀 RAG-Enhanced Functional Requirement (FR) Extraction System

## 📖 Overview

This repository contains the implementation of a **Retrieval-Augmented Generation (RAG) system** for **Functional Requirement (FR) extraction** from unstructured stakeholder inputs.  

The system integrates:

1. **Sentence-BERT embeddings** (`all-MiniLM-L6-v2`) for semantic representation of user stories and use cases.
2. **ChromaDB vector database** to store 1,000+ examples for semantic retrieval.
3. **Gemini API (LLM)** for generating formal SRS statements using augmented prompts from retrieved examples.
4. **RAG pipeline** to improve accuracy, traceability, and domain adaptation.

---

## 🎯 System Architecture

User Input Document → 
  ↓
Semantic Retrival (ChromeDB) → 
  ↓
Retrieve Top-3 Most Similar Examples → 
  ↓
Augmented Prompt Construction → 
  ↓
LLM (Gemini API) → Structured Functional Requirements (FR)

