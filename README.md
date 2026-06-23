# Conversational RAG Knowledge Assistant

A Retrieval-Augmented Generation (RAG) chatbot that allows users to chat with their own knowledge base using natural language.

The application processes documents, stores embeddings in a vector database, retrieves relevant context for user queries, and generates accurate responses using a Large Language Model (LLM).

## Features

* Conversational chat interface
* Retrieval-Augmented Generation (RAG)
* Document ingestion and chunking
* Vector search with ChromaDB
* Hugging Face embedding models
* Fast inference using Groq
* Gradio web interface
* Persistent knowledge base

## Tech Stack

* Python
* LangChain
* ChromaDB
* Hugging Face Embeddings
* Groq API
* Gradio

## Project Structure

```text
.
├── data/
├── vectorstore/
├── app.py
├── requirements.txt
├── .env
└── README.md
```

## Installation

### Clone the repository

```bash
git clone https://github.com/your-username/conversational-rag-knowledge-assistant.git
cd conversational-rag-knowledge-assistant
```

### Create a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

## Environment Variables

Create a `.env` file:

```env
GROQ_API_KEY=your_api_key_here
```

## Running the Application

```bash
python app.py
```

The Gradio interface will start locally and can be accessed through your browser.

## How It Works

1. Documents are loaded from the knowledge base.
2. Text is split into chunks.
3. Chunks are converted into embeddings.
4. Embeddings are stored in ChromaDB.
5. User questions are converted into embeddings.
6. Relevant chunks are retrieved.
7. Context is sent to the LLM.
8. The assistant generates an answer grounded in the retrieved documents.

## Example Use Cases

* Internal company knowledge bases
* Personal note assistants
* Documentation search
* Research assistants
* Learning companions

## Future Improvements

* Multi-document uploads
* PDF support
* Source citations
* User authentication
* Cloud deployment
* Streaming responses

## License

This project is licensed under the MIT License.
