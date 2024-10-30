Here's the full `README.md` file content ready for you to save:

---

# ChatGroq with Llama3 Demo

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
  ```

## Getting Started

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/ChatGroq_Demo.git
cd ChatGroq_Demo
```

### Step 2: Set Up Virtual Environment

Create and activate a virtual environment (recommended).

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

### Step 3: Install Requirements

Install the necessary packages:

```bash
pip install -r requirements.txt
```

### Step 4: Set Up API Keys

1. Create a `.env` file in the project root to securely store your API keys.
2. Add your OpenAI and GROQ API keys in the following format:

   ```plaintext
   OPENAI_API_KEY=your_openai_api_key
   GROQ_API_KEY=your_groq_api_key
   ```

### Step 5: Organize PDF Files

Place the PDF files you wish to analyze in a folder named `pdf_folder` within the project directory.

### Step 6: Run the App

Start the Streamlit app by running:

```bash
streamlit run app.py
```

Open a browser and go to `http://localhost:8501` to interact with the app.

## Usage

1. **Load Document Embeddings**: Click on the "Documents Embedding" button to initialize the vector store.
2. **Ask a Question**: Enter a question in the text input field. The model will generate a response based on the content of the loaded documents.
3. **View Similar Documents**: Use the expander to see document chunks similar to your question.

## Troubleshooting

If you encounter a `RateLimitError` (Error code 429) or an insufficient quota error, please check:
- [Your OpenAI Usage](https://platform.openai.com/account/usage) to ensure you haven't exceeded your quota.
- Ensure valid API keys are set in the `.env` file and that the `dotenv` library is loading them correctly.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions, feel free to reach out to the author via [GitHub Issues](https://github.com/yourusername/ChatGroq_Demo/issues).

---

Replace `https://github.com/yourusername/ChatGroq_Demo.git` and `yourusername` with your actual GitHub repository link and username. Save this as `README.md` in your project directory. Let me know if you need further customization!
