# Enterprise RAG Chatbot

## Overview

An enterprise knowledge assistant built with
Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG).

The system retrieves relevant information from
category-specific knowledge bases and generates
context-aware answers to user queries.

---

## 🎯 Problem

Employees often need to search through internal manuals
and documents to find information related to their work.

The goal of this project is to provide a conversational
interface that can retrieve relevant knowledge and generate
useful answers using an LLM.

---

## 💡 Solution

The chatbot uses a category-aware RAG architecture.

User queries are first classified into a relevant domain,
then the system retrieves documents from the corresponding
vector database before generating an answer with an LLM.

### Supported Categories

- DX
- HR
- Finance
- Food Safety
- ETC

---

## 🏗️ Architecture

```text
User Query
     │
     ▼
Query Classifier
     │
     ├── DX
     ├── HR
     ├── Finance
     └── Food Safety
     │
     ▼
Category-specific Vector DB
     │
     ▼
Document Retrieval
     │
     ▼
LLM
     │
     ▼
Generated Answer
