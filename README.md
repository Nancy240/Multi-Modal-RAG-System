# Multi-Modal RAG System

This repository contains a Jupyter Notebook (`Advanced_RAG.ipynb`) that implements an advanced **Retrieval-Augmented Generation (RAG)** system for processing and querying multi-modal documents, including text, tables, and images. The system leverages LangChain, HuggingFace, and PyTorch to create a pipeline that combines embedding models, a vector store, and a large language model to answer questions based on provided context.

## Project Overview
The notebook builds a RAG system capable of:
- Generating embeddings for text, table, and image summaries using the `sentence-transformers/all-MiniLM-L6-v2` model.
- Storing embeddings in a Chroma vector store and original content in a document store.
- Using the `mistralai/Mistral-7B-Instruct-v0.2` model for generating answers.
- Supporting interactive question-answering with source document retrieval.

The system processes 8 text summaries and 11 image summaries (no table summaries in the example) and demonstrates querying capabilities, such as summarizing a PDF's content.

## Prerequisites
To run the notebook, you need:
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- GPU (optional, for faster model inference)

### Required Libraries
Install the required dependencies using the following command:
```bash
pip install langchain transformers torch sentence-transformers chromadb
