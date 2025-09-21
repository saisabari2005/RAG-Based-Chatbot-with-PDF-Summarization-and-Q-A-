# RAG-Based Chatbot with PDF Summarization and Q&A 🤖📚

A **Retrieval-Augmented Generation (RAG) chatbot** that can summarize PDFs and answer questions using both uploaded documents and prior context. Built with **Streamlit**, **LangChain**, **Groq**, **FAISS**, and **HuggingFace Embeddings**.

---

## Features

- **PDF Summarization**: Generate concise (~100 words) and detailed (~1000 words) summaries of uploaded PDFs.
- **Q&A Chatbot**: Ask questions based on uploaded documents and receive context-aware responses.
- **RAG Integration**: Combines document retrieval with generative AI for accurate answers.
- **Session Management**: Maintains chat history within the session.
- **Vector Storage**: Stores document embeddings locally with FAISS for efficient retrieval.
- **Customizable Prompts**: Use chat prompt templates for consistent, accurate answers.
- **Dynamic Styling**: Enhanced Streamlit UI with gradient-based chat bubbles and responsive design.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/RAG-Chatbot-PDF.git
   cd RAG-Chatbot-PDF
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Required libraries:
   - streamlit
   - langchain
   - langchain-groq
   - langchain-community
   - langchain-huggingface
   - langchain-google-genai
   - PyPDF2
   - numpy
   - sentence-transformers
   - dotenv

---

## Usage ▶️

1. Run the Streamlit app:
   ```bash
   streamlit run part.py
   ```

2. Upload a PDF to summarize or chat with your own data.
3. Ask questions in the chat interface; AI responses are context-aware.
4. Use the "Clear Chat" button to reset the session.

---

## Project Structure 📂

```
├── part.py                  # Streamlit app for summarization and Q&A
├── fullrag.py               # Advanced RAG-based chatbot script
├── requirements.txt         # Python dependencies
├── .env                     # Environment variables (API keys)
└── README.md                # Project documentation
```

---

## How It Works ⚙️

1. **PDF Text Extraction**: Extract text from uploaded PDFs using PyPDF2 or PyMuPDF.
2. **Text Chunking**: Split text into smaller chunks for embedding.
3. **Embeddings**: Generate vector embeddings using GoogleGenerativeAI or HuggingFace models.
4. **Vector Storage**: Store embeddings in FAISS for similarity search.
5. **RAG Q&A**: Retrieve relevant chunks based on user questions and generate answers with ChatGroq.
6. **Streamlit Interface**: Display chat messages and AI responses with a styled, user-friendly UI.

---

## Future Improvements 🚀

- Add multi-language support.
- Integrate other generative models for summarization.
- Add persistent database storage for long-term session management.
- Improve PDF preprocessing for tables, images, and complex layouts.

---

## License 📄

This project is licensed under the MIT License

