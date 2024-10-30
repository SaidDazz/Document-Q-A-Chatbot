# Document-Q-A-Chatbot
## ChatGroq with Llama3 Demo

This project is a chatbot demo application built with Streamlit, using LangChain and the Llama3 language model via the ChatGroq API. It also integrates document embeddings through OpenAI embeddings, allowing for document similarity search on PDF files.

## Features
- **ChatGroq Integration**: Uses the Llama3 language model via ChatGroq to generate responses based on input queries.
- **OpenAI Embeddings**: Supports document embeddings for better similarity search and retrieval.
- **PDF Document Loader**: Loads documents from a specified folder and processes them for embedding.
- **Interactive UI**: Built with Streamlit, providing an easy-to-use web interface.

## Requirements

To set up and run this project, you’ll need:
- Python 3.7 or above
- `requirements.txt` with the following packages:
  ```plaintext
  streamlit
  langchain
  langchain_groq
  langchain_openai
  langchain_core
  langchain_community
  faiss-cpu
  python-dotenv
