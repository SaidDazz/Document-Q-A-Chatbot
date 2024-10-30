# Document Q&A Chatbot using Llama3,Langchain and Groq API

## Overview
A chatbot application built with Streamlit that leverages the LangChain library and the Llama3 language model via the ChatGroq API. It integrates document embeddings using OpenAI's API to enable similarity search on PDF documents.

## Project Description
This project is designed to allow users to ask questions based on the content of uploaded PDF documents. The application splits and embeds these documents, using OpenAI embeddings for document similarity and retrieval. Through a simple user interface built with Streamlit, users can:
- Load PDF documents.
- Create and store embeddings in a vector database.
- Query the Llama3 model to retrieve document-based responses.

## Technologies
- **Streamlit**: For the web-based user interface.
- **LangChain**: A library that supports interaction with large language models.
- **ChatGroq API**: For accessing the Llama3 language model.
- **OpenAI Embeddings**: For document similarity search.
- **FAISS**: For vector storage and retrieval.
- **dotenv**: For managing environment variables securely.

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/ChatGroq_Demo.git
   cd ChatGroq_Demo
   ```

2. **Set Up Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install Required Packages**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up API Keys**
   - Create a `.env` file in the project root.
   - Add your OpenAI and GROQ API keys in this format:
     ```plaintext
     OPENAI_API_KEY=your_openai_api_key
     GROQ_API_KEY=your_groq_api_key
     ```

5. **Organize PDF Files**
   - Place the PDF documents in a folder named `pdf_folder` within the project directory.

## Execution

1. **Run the Streamlit App**
   ```bash
   streamlit run app.py
   ```

2. **Using the Application**
   - Open the app in your browser at `http://localhost:8501`.
   - Click "Documents Embedding" to prepare the vector store.
   - Enter a question related to the PDF documents, and view the model's response and related document snippets.

## Author
- DAZZAZI Ahmed Said - Data Engineer - [GitHub](https://github.com/SaidDazz)

---
