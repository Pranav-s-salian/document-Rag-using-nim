# 📄 Document RAG with NVIDIA NIM 🚀

![NVIDIA NIM Banner](https://developer.nvidia.com/sites/default/files/akamai/ai/images/nim-banner.png)

Welcome to **Document RAG (Retrieval-Augmented Generation) powered by NVIDIA NIM**!  
This project lets you upload your PDF documents, embed them using state-of-the-art NVIDIA embeddings, and ask questions to get instant, context-aware answers using Llama 3 and the NVIDIA NIM platform.

---

## 🌟 Features

- **PDF Upload:** Easily upload multiple PDF files.
- **Automatic Chunking:** Documents are split into manageable chunks for efficient retrieval.
- **NVIDIA Embeddings:** Uses NVIDIA's powerful embedding models for vectorization.
- **FAISS Vector Store:** Fast and scalable similarity search.
- **Llama 3 via NVIDIA NIM:** Advanced language model for accurate, context-based answers.
- **Streamlit UI:** Simple, interactive web interface.

---

## 🛠️ Tech Stack

| Technology                | Purpose                                      |
|---------------------------|----------------------------------------------|
| **Streamlit**             | Web UI for uploading files and asking queries|
| **LangChain**             | Orchestrates document loading, splitting, and retrieval |
| **NVIDIA NIM**            | Provides LLM (Llama 3) and Embeddings APIs  |
| **FAISS**                 | Efficient vector similarity search           |
| **PyPDFDirectoryLoader**  | Loads and parses PDF files                   |
| **Python**                | Core programming language                    |

---

## 🖼️ How It Works

1. **Upload PDFs:**  
   ![Upload PDF](https://img.icons8.com/fluency/96/upload.png)  
   Use the Streamlit interface to upload your PDF documents.

2. **Embedding:**  
   The PDFs are split into chunks and embedded using NVIDIA's Embeddings API via NIM.

3. **Vector Store:**  
   Chunks are stored in a FAISS vector database for fast similarity search.

4. **Ask Questions:**  
   Enter your question. The app retrieves the most relevant document chunks and sends them, along with your question, to Llama 3 (via NVIDIA NIM) for an answer.

5. **Get Answers:**  
   The answer is displayed, along with the most relevant document excerpts for transparency.

---

## 🧩 Code Overview

- **main.py:**  
  - Handles file upload and temporary storage.
  - Loads and splits PDFs.
  - Embeds document chunks using NVIDIAEmbeddings.
  - Stores vectors in FAISS.
  - Uses LangChain to retrieve relevant chunks and generate answers with ChatNVIDIA (Llama 3).
  - Displays answers and supporting document context.

---

## 🟢 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/document-rag-nvidia-nim.git
cd document-rag-nvidia-nim