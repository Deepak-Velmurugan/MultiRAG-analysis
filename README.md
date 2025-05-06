# Hybrid RAG Evaluation System

![RAG Architecture Diagram](https://miro.medium.com/v2/resize:fit:1400/1*9h-WRgVoY5hYJqYezj1RMA.png)

A comparative evaluation framework for Naive RAG, Graph RAG, and Hybrid RAG approaches, combining vector similarity search with graph-based relationship traversal.

## Features

- **Multi-Model RAG Evaluation**: Compare Naive, Graph, and Hybrid RAG systems
- **Hybrid Retrieval**: Combines ChromaDB vector search with Neo4j graph traversal
- **Comprehensive Metrics**: Precision@K, Recall@K, F1, BLEU, latency, and memory usage
- **Document Processing**: Supports PDF and text files with automatic chunking
- **Interactive UI**: Streamlit-based dashboard with visualizations

## Architecture
NaiveRAG:
![image](https://github.com/user-attachments/assets/5b072093-3067-4c28-8900-c0d5d4a4d847)

##
Evaluation Metrics
Metric	Description
Precision@K	% of relevant chunks in top K results
Recall@K	% of all relevant chunks retrieved
F1 Score	Harmonic mean of precision and recall
BLEU Score	Language generation quality
Latency	Retrieval and generation times
Memory	System resource usage
