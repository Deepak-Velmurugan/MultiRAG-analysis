# Hybrid RAG Evaluation System
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

GraphRAG
![image](https://github.com/user-attachments/assets/1a02320e-dcf7-474a-b6c2-b9568d29a9e1)

HybridRAG
![image](https://github.com/user-attachments/assets/4ef5f3af-fffb-4fe9-aab8-2b8fbfee26da)

##
Evaluation Metrics
Metric	        Description
Hallucination   Assessing whether information unsupported by retrieved context is introduced in the answer. 
Precision@K	    Fraction of retrieved chunks that are relevant to the query 
Recall@K	      Fraction of relevant chunks successfully retrieved among all relevant chunks
F1 Score	      Harmonic mean of precision and recall
BLEU Score	    Language generation quality
Latency	        End-to-end time from query submission to answer generation
Memory	        Peak and average memory usage during retrieval and generation
