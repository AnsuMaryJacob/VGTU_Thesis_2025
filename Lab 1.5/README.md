# AI-Enabled Requirements Engineering Agent – Prompt Documentation

This directory contains prompt examples and implementation notes for the AI-Enabled Requirements Engineering Specification (RES) system.Each prompt demonstrates how the RAG-based AI agent processes input data X (stakeholder statement) to generate a structured output y (SRS-formatted requirement).

## ✨ Key Features

- Uses Retrieval-Augmented Generation (RAG) logic with prompt-based reasoning.  
- Demonstrates both **Zero-Shot** and **Few-Shot** prompt engineering techniques.  
- Integrates securely with the Gemini API via a secret key in Colab.  
- Outputs clear, traceable requirements (FR/NFR) from natural language input.

## 🎯 System Overview

You are an AI-enabled Requirements Engineering Agent that combines Retrieval-Augmented Generation (RAG) with a BERT-based requirement classifier.
Your objective is to transform unstructured stakeholder statements into clear, traceable, and testable software requirements.

## ⚙️ Pipeline Components
| Stage                                     | Description                                                                                                   |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Text Preprocessing & Normalization | Cleans and standardizes stakeholder inputs.                                                                   |
| Context Retrieval (via FAISS)      | Finds relevant content from a domain knowledge base (e.g., banking/chatbot dataset).                          |
| Requirement Classification (BERT)  | Distinguishes **Functional (FR)** vs. **Non-Functional (NFR)** requirements using a Sentence-BERT classifier. |
| Formal Requirement Generation      | Generates standardized SRS statements starting with: *“The system shall …”* using FLAN-T5 or Gemini.          |

## ⚙️ Notebook
Link to Colab document: https://colab.research.google.com/drive/1S8p5KFxncKA7-6nimLjC7yFckin23lNQ#scrollTo=R-qt8A-MvCfg

## 🛠️ Technology Stack ===============================

Language: Python 3

LLM (Generation & Reasoning) : Google Gemini 1.5 Pro → Used in your Colab notebook to generate SRS requirements.

Requirement Classification

Sentence-BERT (SBERT) : Used to classify requirements into FR / NFR.

Text Generation

FLAN-T5 or GPT-based models (optional local models) : Converts structured features into formal requirement statements.

Retrieval-Augmented Generation (RAG) Layer

FAISS (Facebook AI Similarity Search) : Vector store for fast semantic search.Retrieves similar statements or domain knowledge.

Sentence-BERT Embeddings : Used to encode stakeholder inputs and knowledge base entries.

Data & Storage

Knowledge Base for Domain Context (Banking/Chatbot domain) : Stored as text files, JSON, or CSV, Embedded using SBERT

Vector Store (FAISS Index) : Stores document embeddings for fast retrieval.

Local Dataset: Raw stakeholder inputs, Annotated FR/NFR classification files, Sample SRS outputs

## 📈 Summary and Reflection
# 🧭 Reflection

This end-to-end demonstration showcases how the AI-Enabled Requirements Engineering Agent operates within a Gemini-based reasoning pipeline.

**System Behavior:**
- Accepts unstructured stakeholder statements (X)
- Uses contextual and semantic reasoning (RAG + BERT logic)
- Outputs standardized Software Requirement Specifications (SRS)

**Gemini & Prompt Engineering Usage:**
- Gemini provides reasoning, linguistic clarity, and format consistency.
- Zero-Shot prompt tests generalization ability.
- Few-Shot prompt leverages examples for improved accuracy.

**Observations:**
- Few-Shot prompting yielded more domain-aligned outputs.
- Zero-Shot handled new contexts effectively.
- Future improvements: integrate FAISS for real retrieval + classifier fine-tuning.


engineering was used in both a zero-shot capacity for direct extraction and a few-shot capacity where examples were provided to improve the model's performance on a new task.
