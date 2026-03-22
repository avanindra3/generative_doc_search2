# Generative Doc Search

This is a generative search system capable of effectively and accurately answering questions from a Group Member Life Insurance Policy document using LlamaIndex.

## 1. Requirements
The system relies on several core Python libraries for document processing, vector storage, and language model interaction:
- `llama-index` (RAG Framework)
- `chromadb` (Vector Database)
- `openai` (LLM Provider)
- `sentence-transformers` (Reranking Model)

## 2. Environment Setup
Install the necessary dependencies using the following command:
```bash
pip install llama-index chromadb openai sentence-transformers
```

## 3. File System & Configuration
Ensure your project root is structured as follows for the ingestion pipeline to function correctly:

- **'data/' Directory:** Create a folder named `data` in the root directory and place all insurance PDF documents (e.g., policy handbooks, claim forms) inside it.
- **'storage/' Directory:** Create a folder named `storage` in the root directory for ChromaDB database.
- **'openai_api_key.json':** Create a JSON file in the root directory to store your API credentials. The file must follow this exact format:
  ```json
  {
    "api_key": "YOUR_KEY_HERE"
  }
  ```

## 4. Running the System
Once the libraries are installed and the files are in place, you can execute the notebook cells sequentially to initialize the database, build the index, and begin querying the insurance documents.
