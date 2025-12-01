# MASTER'S THESIS - LAB WORKS INTEGRATION MAP
## AI-Enabled Requirements Engineering Specification Using RAG

---

## LAB 01: Automated Thesis Synthesis and Multimedia Content Generation(NotebookLM)
### What Was Done:
- Uploaded thesis draft and 3 key scientific papers to NotebookLM
- Video overview, Audio overview, Reports, Flashcards and MindMap
- Automated summarization of contextual studies.

### Key Contributions to Your Thesis
- Defining the Problem Statement and Research Gap :- The sources explicitly highlight the core problem your thesis must address: the difficulty of specifying requirements for probabilistic AI/ML models and the need for new methods to achieve explainability.
- Structuring the Literature Review :- The systematic mapping provides a natural way to organize your Literature Review chapter.
- Providing Technical Components for Your Approach :- The sources give you specific, cutting-edge AI techniques to incorporate into the design of your novel approach.

```
Technique  →    Source Context  → Thesis Integration Role
─────────────────────────────────────────────────
Transformer Models (e.g., BERT)        →    Automated NFR Classification  → Foundation: Supports automated reading and structuring of textual requirements.
Knowledge Graphs (KG)   →    Multimodal data fusion for diagnosis  → Structure: Provides a formal, traceable, and interconnected model for requirements, constraints, and design rationale.
Retrieval-Augmented Generation (RAG)   →    Generating dependable explanations  → Verification & Explanation: Ensures system output (requirements, documentation, rationale) is grounded in authoritative sources, boosting reliability and meeting the need for explainability.

```
## LAB 02: End-to-End AI-Driven RE Solution and Process Modeling
- Created (X, y) examples:
  * X = Chatbot input from the customer/ person 
  * y = Extracted functional requirements

### Key Contributions to Your Thesis
- The need to automate elicitation, analysis, and formalization from unstructured natural language is the problem statement. The goal is a validated, structured SRS.
- The Examples of (X, y) Pairs are the empirical data used for training and testing, which will be referenced here.
- The proposed areas (Predictive Quality, Anomaly Detection, Process Mining) represent high-value, research-worthy extensions to your novel approach.

## LAB 03: UML System Design and GAI Integration
- Identified  a firm : A retail Babk (swedbank lithuania)
- Created UML diagrams using PlantUML + LLM assistance:
  * Class Diagram
  * Component Diagram
  * Sequence Diagram
  * Activity Diagram
- Showed GAI integration architecture

### Key Contributions to Your Thesis
- The thesis now promises practical benefits for the bank, such as automated requirement extraction from chat logs, improved compliance traceability, and faster drafting of the Software Requirements Specification (SRS).
- The Sequence Diagram and Activity Diagram provide a step-by-step methodology for the system's operation, from collecting chat transcripts and anonymizing text to the final storage in the SRS Repository.
- The Requirement class includes the attribute provenance (a list of chunkIds), solidifying how the solution maintains traceability back to the raw stakeholder input.

## LAB 04: AI Agent Conceptualization and Prompt Engineering
- Conceptualized thesis system as single AI agent
- Created `/prompts/` directory in GitHub
- Developed 2 core prompts:
  * Prompt 1: Zero-shot FR extraction
  * Prompt 2: Few-shot with examples
 
### Key Contributions to Your Thesis
- It provides a specific, sequential breakdown of the AI Processing Layer steps, which forms the core of your methodology: Text Preprocessing, Context Retrieval (via FAISS), Classification (using Sentence-BERT), and Formal Generation (using FLAN-T5 or GPT-based model).
- It mandates the use of the industry-standard requirement format, "The system shall...", confirming that your novel approach generates formal, standardized SRS statements.
- The process confirms that Contextual Retrieval is performed against a domain-specific knowledge base (e.g., banking operations), demonstrating how the system provides grounded, relevant output.

## LAB 05: End-to-End Implementation (Google Colab + Gemini API)
- Completed the full system implementation within a Google Colab environment.
- Engineered a functional prototype, leveraging the Gemini API for core Large Language Model (LLM) operations.
- Developed a well-structured, executable prototype notebook containing operational code, descriptive analysis, and two verified prompt examples.
- Successfully deployed the entire RAG pipeline and model processing logic using the Gemini API within a Colab notebook.

### Key Contributions to Your Thesis
- The successful implementation of the complete pipeline in Google Colab confirms the technical feasibility of your novel approach. This moves the thesis from a conceptual model (UML diagrams) to a concrete, executable system.
- The successful use of the Gemini API for LLM processing validates the choice of using a specific, powerful generative AI model to handle the complex requirement generation and refinement tasks.
- The few-shot example demonstrates the agent's ability to learn formatting and structural patterns from minimal input, which is crucial for generating formalized, standardized requirements (e.g., using "The system shall...")
- The zero-shot example proves the agent's capability to apply its learned rules and context (from the RAG knowledge base) to generate coherent, novel requirements from a single, unseen stakeholder input.

## LAB 06: Advanced Evaluation and Visualization
- Expanded evaluation beyond Lab 05's manual checks
- Implemented automated metrics (RAGAS-based)
- Created comprehensive visualizations

### Key Contributions to Your Thesis
- RAGAS provides specialized metrics (like Faithfulness, Context Relevance, and Answer Recall) that are specifically designed to evaluate the performance and quality of the Retrieval-Augmented Generation (RAG) pipeline—the core of my novel approach.
- Creating comprehensive visualizations (e.g., error rate graphs, metric comparisons, performance benchmarks) allows  to summarize and highlight the system's strengths and weaknesses more effectively than raw data or simple tables.
- Having a strong, automated metric framework ensures that the conclusions and claims made in your thesis regarding the effectiveness and quality of  AI-Driven Requirements Specification Approach are defensible and backed by objective data.

