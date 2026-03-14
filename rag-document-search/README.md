# RAG Document Search Pipeline

This project demonstrates a simple **Retrieval-Augmented Generation (RAG)** pipeline for answering questions using information retrieved from a document.

## Objective

Build a system that retrieves relevant document sections and uses them as context for generating answers with a language model.

## Architecture

```
Document → Chunking → Embeddings → Vector Database → Retrieval → LLM Answer
```

## Workflow

1. Load a source document
2. Split the document into manageable chunks
3. Convert text chunks into embeddings
4. Store embeddings in a FAISS vector database
5. Retrieve relevant chunks based on a user query
6. Generate an answer using the retrieved context

## Tools Used

* Python
* LangChain
* HuggingFace Embeddings
* FAISS Vector Store
* Google Colab

## Notebook

The full implementation is available in:

```
rag_document_search_pipeline.ipynb
```

## Example Use Case

This type of system is commonly used for:

* document question answering
* customer support assistants
* internal knowledge search
* policy and legal document retrieval
