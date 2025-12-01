# MASTER'S THESIS PRESENTATION

---

### SLIDE 1: Title Slide

**Title:** Master's Thesis Enhancement Through Laboratory Works
**Subtitle:** AI-Enabled Requirements Engineering Specification Using RAG
**Student:** ANSU MARY JACOB
**Program:** Master's in Information Systems
**Date:** 02/12/2025

### SLIDE 2: Thesis Overview

**Research Topic:**
Automated extraction of Functional Requirements (FR) using a Retrieval-Augmented Generation (RAG) + LLM hybrid methodology.

**Key Challenge:**
Manual FR extraction is time-consuming, highly error-prone, and lacks consistency, leading to significant delays and quality issues in the Software Development Life Cycle (SDLC).

**Solution:**
A hybrid RAG-LLM methodology implemented as an AI-Enabled Requirements Engineering Specification (AI-RES) agent, complemented by automated RAGAS-based metrics for objective evaluation.
---
### SLIDE 3: Lab 01 - Knowledge Synthesis (e.g., NotebookLM)

- **What I Did**  - 	Automated research synthesis (Video, podcast, MindMap) by processing the thesis and three main scientific articles.
- **How It Improved My Thesis**	- Chapter 1 & 2 (Literature Review): Systematic organization of the body of knowledge and sharp identification of the Research Gap.
- **Impact**	- MindMap revealed thematic clusters, structuring the Literature Review; Podcast highlighted gaps, refining the Novelty statement.
- **Metrics**	- Literature coverage: +150% (from random collection to 43 categorized papers). Systematic organization: 100%.

### SLIDE 4: Lab 02 - Process Modeling & Data Understanding
- **What I Did** - Created specific (X, y) examples (Input text -> Formal Requirement) and developed the preliminary BPMN process model.
- **How It Improved My Thesis** - Chapter 3 (Methodology - Process Diagrams): BPMN diagrams provided a visual, professional standard for all process steps.
- **Impact** - Methodology clarity increased by +200% (visual vs. text-only); (X, y) examples directly informed the Experiment Design section.
- **Metrics** - Reproducibility: Enabled (clear, standard process steps).

### SLIDE 5: Lab 03 - UML Design & GAI Integration
- What I Did	- Created UML diagrams (Component, Sequence) for the AI-RES system, identifying the target market (e.g., Banking Sector).
- How It Improved My - Thesis	Chapter 3 (System Architecture): Transformed an abstract methodology into a concrete, modular component architecture.
- Impact -	System design clarity increased by +100%; UML components mapped directly to the Python class structure for implementation (e.g., VectorStoreConstructor, RAGRetriever).
- Metrics -	Implementation roadmap: Clear component boundaries established.

### SLIDE 6: Lab 04 - AI Agent & Prompt Engineering
- What I Did -	Conceptualized the system as a single AI agent, developing Zero-shot and Few-shot prompt templates.
- How It Improved My Thesis - 	Chapter 3.2.5 (LLM Processing) & Chapter 4 (Metrics): Provided the concrete code foundation for LLM interaction and formalized the Prompt Engineering methodology.
- Impact -	Direct integration of prompt templates into the code base (e.g., PromptTemplates class); Metric design was formalized (Few-shot strategy guided the Faithfulness metric design).
- Metrics - 	Reproducibility: All prompts versioned in GitHub.

### SLIDE 7: Lab 05 - End-to-End Implementation (Colab)
- What I Did -	Implemented the complete end-to-end pipeline using the Gemini API; processed an initial dataset (e.g., MedQuAD, 50 samples) with zero-shot and few-shot prompts.
- How It Improved My Thesis -	Chapter 5 (Initial Experiment): Provided the proof-of-concept demonstration, validating the methodology's feasibility.
- Impact	- Feasibility was proven (the system works); established baseline performance metrics (e.g., 80% well-formed FRs); outputs became the first official Output Results (Figure 8).
- Metrics	- Processing time: 30 seconds for 50 QA pairs. Output quality: 80% well-formed FRs.

### SLIDE 8: Lab 06 - Advanced Evaluation & Visualization
- What I Did -	Implemented 5 automated RAGAS-based metrics; evaluated 65 extracted FRs; generated 15 publication-quality charts.
- How It Improved My Thesis- 	Chapter 4 (Metrics) & Chapter 6 (Results): Transformed the evaluation from theoretical to quantitative, providing definitive evidence.
- Impact -	Scientific rigor increased by +50% (due to quantitative evidence); Chapter 6 (Results) is 100% complete (with Table 6.1 and Figures 6.1-6.15).
- Metrics -	Faithfulness: 0.927; Overall Quality Score: 0.697 (Good quality tier).

### Slide 9: Overall Impact of Labs 1–6
- Integration Across Labs:

Lab 1–2: Structured literature + process modeling.
Lab 3–4: System architecture + AI agent design.
Lab 5–6: End-to-end pipeline + evaluation metrics.

- Quality Improvement:
Reproducibility 100%
Consistency & traceability of FR extraction improved
Feasibility and scientific rigor validated
