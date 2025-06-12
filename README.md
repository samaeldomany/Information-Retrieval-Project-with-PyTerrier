# Information-Retrieval-Project
This project demonstrates core concepts of Information Retrieval (IR) using the PyTerrier framework. It includes data loading, text preprocessing, indexing, and various retrieval models.


## Overview
This Jupyter Notebook provides a comprehensive introduction to Information Retrieval using the PyTerrier library. It covers essential steps such as loading standard IR datasets, preprocessing text (tokenization, lowercasing, stop word removal, stemming), building an inverted index, and performing information retrieval using different weighting models. The project also showcases query expansion using pseudo-relevance feedback (PRF).

## Features
### 1. PyTerrier Integration
- Seamlessly integrates with the PyTerrier framework for efficient IR operations.
- Initializes PyTerrier with PRF capabilities.

### 2. Data Collection and Loading
- Utilizes pt.datasets.get_dataset("vaswani") to load a standard IR dataset, including topics (queries) and qrels (relevance judgments) [cite: uploaded:Sama_Mohamed_202201867.ipynb].

### 3. Text Preprocessing Pipeline
- Tokenization: Breaks down text into individual words or terms [cite: uploaded:Sama_Mohamed_202201867.ipynb].

- Lowercasing: Converts all text to lowercase to ensure case-insensitive matching [cite: uploaded:Sama_Mohamed_202201867.ipynb].

- Stop Word Removal: Eliminates common words (e.g., "the", "a", "is") that do not contribute significantly to meaning [cite: uploaded:Sama_Mohamed_202201867.ipynb].

- Stemming: Reduces words to their root form (e.g., "running" to "run") using Porter Stemmer to normalize terms [cite: uploaded:Sama_Mohamed_202201867.ipynb].

- Preprocessed Queries: Applies the full preprocessing pipeline to search queries [cite: uploaded:Sama_Mohamed_202201867.ipynb].

### 4. Indexing
- Builds an inverted index from the dataset, enabling fast retrieval of documents based on query terms.

- Demonstrates the process of creating and managing the index using PyTerrier.

### 5. Retrieval Models
- Allows for the application of different weighting models (e.g., BM25) to rank documents based on their relevance to a given query.

- Performs search operations and displays ranked results.

6. Query Expansion (Pseudo-Relevance Feedback - PRF)
- Implements PRF techniques (e.g., RM3) to improve retrieval effectiveness by automatically expanding queries based on initial search results [cite: uploaded:Sama_Mohamed_202201867.ipynb].

- Shows how the original query is reformulated and how the expanded query affects search results.

7. Evaluation (Implicit)
- While not explicitly calculating metrics in the provided snippets, the structure sets up for evaluation by using qrels for relevance judgments.
