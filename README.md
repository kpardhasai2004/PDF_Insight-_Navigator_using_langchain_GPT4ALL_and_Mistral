 # PDF Insight Navigator

## Project Overview

This project demonstrates a question-answering system that combines information retrieval with a large language model (LLM) to provide comprehensive and context-aware answers. It leverages LangChain for model chaining and vector databases for efficient text search.

## Key Features

- **Retrieves relevant context from PDF documents:** Uses FAISS vector database for fast similarity search.
- **Generates answers using a large language model:** Employs Mistral-Instruct for human-quality text generation.
- **Incorporates context into answers:** Ensures responses are grounded in relevant information.

## Getting Started

1. Install required libraries:

   ```bash
   !pip install langchain tiktoken faiss-cpu gpt4all pypdf huggingface-hub InstructorEmbedding sentence_transformers vectordb
   ```

2. Download the model:

   ```bash
   !wget https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.1-GGUF/resolve/main/mistral-7b-instruct-v0.1.Q5_K_M.gguf -P models
   ```

3. Run the code

## Usage

1. Load and prepare PDF documents.
2. Create a vector database for efficient text search.
3. Load the LLM and define a prompt template.
4. Ask a question.
5. Retrieve relevant context from the vector database.
6. Generate an answer using the LLM, incorporating the retrieved context.
