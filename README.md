# Ecommerce-taxonomy-pipeline
An end-to-end data science pipeline for eCommerce taxonomy gap analysis, LLM-based data enrichment, and semantic search (RAG) using the Amazon ESCI dataset.

# eCommerce Taxonomy Enrichment & Semantic Search Pipeline

An end-to-end machine learning and LLM engineering pipeline designed to audit eCommerce catalog data, automate product taxonomy enrichment via structured prompt workflows, deploy vector-based semantic search (RAG), and benchmark classification performance using industry evaluation metrics.

Built with real-world catalog samples from the **Amazon ESCI (Shopping Queries) Dataset** to simulate core Knowledge Management and catalog ontology challenges at marketplace scale.

---

## 🏗️ Architecture & Pipeline Overview

```text
Raw Catalog Data (ESCI)
          │
          ▼
[Phase 1: Catalog Gap Analysis] ──► Identified 124,858 missing brands & malformed descriptions
          │
          ▼
[Phase 2: LLM Taxonomy Enrichment] ──► Few-Shot Prompt Engineering -> Strict JSON extraction
          │
          ▼
[Phase 3: Semantic Search & RAG] ──► ChromaDB Vector Store (`all-MiniLM-L6-v2`) + LLM Assistant
          │
          ▼
[Phase 4: Quantitative Evaluation] ──► Macro F1, Precision, Recall & Misclassification Error Analysis
