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

<div align="center">

<table>
  <tr>
    <td align="center">
      <img src="https://streamlit.io/images/brand/streamlit-logo-primary-colormark-darktext.png" width="80"/><br>
      <b>Streamlit</b>
    </td>
    <td align="center">
      <img src="https://avatars.githubusercontent.com/u/139895814?s=200&v=4" width="80"/><br>
      <b>LangChain</b>
    </td>
    <td align="center">
      <img src="https://developer.nvidia.com/sites/default/files/akamai/ai/images/nim-banner.png" width="80"/><br>
      <b>NVIDIA NIM</b>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/facebookresearch/faiss/main/resources/faiss-logo.png" width="80"/><br>
      <b>FAISS</b>
    </td>
    <td align="center">
      <img src="https://img.icons8.com/ios-filled/100/pdf.png" width="60"/><br>
      <b>PyPDFDirectoryLoader</b>
    </td>
    <td align="center">
      <img src="https://www.python.org/static/community_logos/python-logo.png" width="80"/><br>
      <b>Python</b>
    </td>
  </tr>
</table>

</div>

---

<div align="center">

| <b>Technology</b>           | <b>Purpose</b>                                                      |
|-----------------------------|---------------------------------------------------------------------|
| Streamlit                   | Web UI for uploading files and asking queries                       |
| LangChain                   | Orchestrates document loading, splitting, and retrieval             |
| NVIDIA NIM                  | Provides LLM (Llama 3) and Embeddings APIs                         |
| FAISS                       | Efficient vector similarity search                                  |
| PyPDFDirectoryLoader        | Loads and parses PDF files                                          |
| Python                      | Core programming language                                           |

</div>

---

## 🖼️ How It Works

1. <b>Upload PDFs</b>  
   <div align="center"><img src="https://img.icons8.com/fluency/96/upload.png" width="60"/></div>  
   Use the Streamlit interface to upload your PDF documents.

2. <b>Embedding</b>  
   The PDFs are split into chunks and embedded using NVIDIA's Embeddings API via NIM.

3. <b>Vector Store</b>  
   Chunks are stored in a FAISS vector database for fast similarity search.

4. <b>Ask Questions</b>  
   Enter your question. The app retrieves the most relevant document chunks and sends them, along with your question, to Llama 3 (via NVIDIA NIM) for an answer.

5. <b>Get Answers</b>  
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
cd document-rag-nvidia-
