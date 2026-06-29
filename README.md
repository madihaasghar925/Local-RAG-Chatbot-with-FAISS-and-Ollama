#  Local RAG Chatbot

A Retrieval-Augmented Generation (RAG) chatbot that allows users to ask questions from their own documents using local Large Language Models.

The application processes documents, converts them into vector embeddings, stores them in a FAISS index, and retrieves the most relevant information before generating responses using Ollama.

---

##  Features

-  Scan an entire folder of documents
-  Automatic text chunking
-  Generate embeddings using Sentence Transformers
-  Fast similarity search using FAISS
-  Save and reload embeddings
-  Local LLM inference with Ollama
-  Interactive Streamlit interface
-  Runs completely offline (after model download)

---

##  Tech Stack

- Python
- Streamlit
- FAISS
- Sentence Transformers
- Ollama
- LangChain (if used)
- NumPy

---

##  Project Structure

```
project/
│
├── app.py                 # Streamlit UI
├── main.py                # Core RAG functions
├── requirements.txt
├── README.md
├── embeddings/
├── documents/
└── faiss_index/
```

---

##  Workflow

```
Documents
      │
      ▼
Text Extraction
      │
      ▼
Chunking
      │
      ▼
Sentence Transformer Embeddings
      │
      ▼
FAISS Vector Store
      │
      ▼
User Query
      │
      ▼
Similarity Search
      │
      ▼
Relevant Chunks
      │
      ▼
Ollama LLM
      │
      ▼
Generated Answer
```

---

##  Installation

Clone the repository

```bash
git clone https://github.com/yourusername/local-rag-chatbot.git

cd local-rag-chatbot
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

##  Run Ollama

Make sure Ollama is installed.

Pull the required model

```bash
ollama pull llama3
```

Start Ollama

```bash
ollama serve
```

---

##  Run the Project

```bash
streamlit run app.py
```

---

##  How It Works

1. Place your documents inside the target folder.
2. The application scans all files.
3. Text is split into manageable chunks.
4. Embeddings are generated using Sentence Transformers.
5. Embeddings are stored in a FAISS vector database.
6. User asks a question.
7. Relevant chunks are retrieved.
8. Ollama generates the final answer using retrieved context.

---

##  Future Improvements

- PDF support
- DOCX support
- Conversation memory
- Multi-document retrieval
- Citation support
- Chat history
- Multiple LLM selection
- Hybrid search (FAISS)



##  Project Files

Due to GitHub's file size limitations, the complete project package is available here:

 Google Drive:
https://drive.google.com/file/d/1_VQIeBb5aXo7I9abyATQJM-47Txi2JJJ/view?usp=drive_link

The repository contains the complete source code, while large files and assets are available through the Drive link if needed.

