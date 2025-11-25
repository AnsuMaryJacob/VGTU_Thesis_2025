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

User Input Document 
  ↓
Semantic Retrival (ChromeDB) 
  ↓
Retrieve Top-3 Most Similar Examples 
  ↓
Augmented Prompt Construction 
  ↓
LLM (Gemini API) → Structured Functional Requirements (FR)


- Semantic retrieval finds the most relevant examples in the database to guide the LLM.
- Augmented prompts reduce hallucinations and improve domain-specific terminology usage.

---

## ⚡ Features

- **Context-aware FR generation** using RAG
- **Domain adaptation** for healthcare, finance, e-commerce, etc.
- **Traceability and compliance tagging** (HIPAA, HL7, safety rules)


## ⚙️ Notebook
Link to Colab document: https://colab.research.google.com/drive/1hB2iisWrEnPLvMhLpHevG5aZtengMLyw#scrollTo=p4xe5-0nYfw_
- **Batch embedding generation** for scalability
- **Colab-ready notebook** with step-by-step demonstration

## 📝 Summary & Reflection

### Summary
This lab demonstrates a **RAG-enhanced Functional Requirement (FR) extraction system** using Sentence-BERT embeddings, ChromaDB vector storage, and the Gemini API for LLM processing. The system:

- Accepts unstructured stakeholder inputs (user stories, interviews, use cases)  
- Encodes inputs and 1,000+ training examples into semantic embeddings  
- Stores embeddings in ChromaDB for fast, similarity-based retrieval  
- Retrieves the top-3 semantically similar examples for each new input  
- Constructs an augmented prompt with examples for the Gemini API  
- Generates structured, traceable, and testable functional requirements  

### Reflection
- **Improved Accuracy:** RAG retrieval provides context, increasing confidence and reducing hallucinations in FR generation.  
- **Domain Adaptation:** Semantic search ensures outputs use correct domain-specific terminology (e.g., healthcare compliance terms).  
- **Consistency & Traceability:** Augmented prompts guide the LLM to produce FRs following the same format as examples, improving traceability to source data.  
- **Scalability:** The system can handle thousands of examples; adding more examples continuously improves performance without retraining the LLM.  
- **Insights:** RAG integration transformed the system from generic LLM outputs to a **domain-aware assistant**, capable of producing high-quality, structured software requirements suitable for real-world use.  
- **Challenges:** Managing metadata for ChromaDB (lists → strings) and handling batch embeddings to prevent memory overload were critical for smooth execution.  

> Overall, the lab illustrates the value of combining **semantic search with LLMs** to create a practical, reliable, and domain-aware AI requirements engineering tool.
