# AI-Enabled Requirements Engineering Agent – Prompt Documentation

This directory contains prompt examples and implementation notes for the AI-Enabled Requirements Engineering Specification (RES) system.Each prompt demonstrates how the RAG-based AI agent processes input data X (stakeholder statement) to generate a structured output y (SRS-formatted requirement).

## ✨ Key Features=================================

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
| **1. Text Preprocessing & Normalization** | Cleans and standardizes stakeholder inputs.                                                                   |
| **2. Context Retrieval (via FAISS)**      | Finds relevant content from a domain knowledge base (e.g., banking/chatbot dataset).                          |
| **3. Requirement Classification (BERT)**  | Distinguishes **Functional (FR)** vs. **Non-Functional (NFR)** requirements using a Sentence-BERT classifier. |
| **4. Formal Requirement Generation**      | Generates standardized SRS statements starting with: *“The system shall …”* using FLAN-T5 or Gemini.          |


## 🛠️ Technology Stack ===============================

Language: Python 3

LLM: Google Gemini (gemini-1.5-pro-latest or similar)

Core Libraries:
google-generativeai: For interacting with the Gemini API.

python-dotenv: For managing environment variables (like API keys).

tabulate: For formatting and displaying metric tables.

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
