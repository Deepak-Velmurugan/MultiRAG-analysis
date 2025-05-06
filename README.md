#MultiRAG Analysis System

A comparative evaluation framework for Naive RAG, Graph RAG, and Hybrid RAG approaches, combining vector similarity search with graph-based relationship traversal.

## Features

- **Multi-Model RAG Evaluation**: Compare Naive, Graph, and Hybrid RAG systems
- **Hybrid Retrieval**: Combines ChromaDB vector search with Neo4j graph traversal
- **Comprehensive Metrics**: Precision@K, Recall@K, F1, BLEU, latency, and memory usage
- **Document Processing**: Supports PDF and text files with automatic chunking
- **Interactive UI**: Streamlit-based dashboard with visualizations

## Architecture

__NaiveRAG__
![image](https://github.com/user-attachments/assets/5b072093-3067-4c28-8900-c0d5d4a4d847)

__GraphRAG__
![image](https://github.com/user-attachments/assets/1a02320e-dcf7-474a-b6c2-b9568d29a9e1)

__HybridRAG__
![image](https://github.com/user-attachments/assets/4ef5f3af-fffb-4fe9-aab8-2b8fbfee26da)

## Evaluation Metrics

- __Hallucination:__  Assessing whether information unsupported by retrieved context is introduced in the answer. 
- __Precision@K:__	  Fraction of retrieved chunks that are relevant to the query 
- __Recall@K:__	      Fraction of relevant chunks successfully retrieved among all relevant chunks
- __F1 Score:__	      Harmonic mean of precision and recall
- __BLEU Score:__	    Language generation quality
- __Latency:__	      End-to-end time from query submission to answer generation
- __Memory:__	        Peak and average memory usage during retrieval and generation

## Requirements
- Python 3.9+
- Neo4j database (optional for Graph/Hybrid RAG)
- Google Gemini API key
- ChromaDB
- Streamlit

## Installation
- Clone the repository:
```bash
git clone https://github.com/Deepak-Velmurugan/MultiRAG-analysis.git
cd MultiRAG-analysis
```
- Create/activate a virtual environment with Python 3.9+:
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```
- Install dependencies
```bash
pip install -r requirements.txt
```
- Set up environment variables:
```bash
cp .env.example .env
```
- Edit .env with your:
  - Google Gemini API key
  - Neo4j credentials (URI, username, password)

## Usage
- Start the Streamlit app:
```bash
streamlit run MultiRAG-Analysis.py
```
## In the browser interface:
- Upload documents (PDF or text)
- Enter your question
- Provide ground truth (optional, for evaluation)
- View comparative results
