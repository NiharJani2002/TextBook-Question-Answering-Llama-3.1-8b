# TextBook-Question-Answering-Llama-3.1-8b

## Who Is The Star of This Project ##
The Star Boy Is Llama 3.1 8b.

The Facebook Recently just like one or two or three days from todays date on which Repo was created (26 Th July 2024)

# PDF Text Extraction and Querying with NLP

This repository contains a script for extracting text from PDF documents, indexing it hierarchically, and performing information retrieval and generation using NLP techniques. The script leverages several libraries including Hugging Face's Transformers, SpaCy, and BM25 for text processing and query generation.

## Overview

The script performs the following tasks:

1. **Text Extraction from PDF**: Extracts text from a PDF document.
2. **Hierarchical Tree-based Indexing**: Processes and indexes the extracted text into a hierarchical structure based on chapters, sections, and subsections.
3. **Retrieval Techniques**: Utilizes BM25 and Dense Passage Retrieval (DPR) models to find relevant documents based on a query.
4. **Retrieval Augmented Generation (RAG)**: Generates a response to a user query using the relevant documents as context.

## Setup

To run the script, you'll need to install several Python packages. Follow the instructions below to set up your environment.

### Prerequisites

- Python 3.x
- `pip` (Python package installer)

### Installation

Run the following commands to install the required libraries:

```bash
pip install torch
pip install --upgrade transformers
pip install accelerate huggingface_hub
pip install pymupdf
pip install spacy
python3 -m spacy download en_core_web_trf
pip install rank_bm25
pip install nltk
python3 -m nltk.downloader wordnet
pip install faiss-cpu
pip install --upgrade pip setuptools wheel
pip install bertopic --no-cache-dir
pip uninstall hdbscan -y
pip install hdbscan --no-cache-dir --no-binary :all: --no-build-isolation


### Hugging Face Authentication ###
from huggingface_hub import login

# Replace 'your_token_here' with your actual Hugging Face token
token = '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'
login(token)

