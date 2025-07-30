# 🤖 PDF Question-Answering Chatbot (Colab + Ollama + LangChain)

This notebook lets you **upload any PDF**, ask questions about its content, and get intelligent responses using a **locally hosted LLaMA 3.1 8B model (via Ollama)**. It uses **LangChain**, **HuggingFace embeddings**, and **Chroma vectorstore** to retrieve accurate answers.

---

## 📌 Features

- Upload any PDF and automatically load its content
- Split text into manageable chunks for embedding
- Embed with `all-MiniLM-L6-v2` from Hugging Face
- Use Ollama’s `llama3:8b` model for local inference
- Ask natural language questions and get answers based only on the PDF context
- Built entirely in **Google Colab** for easy execution

---

## 🧩 Tech Stack

| Component           | Purpose                                 |
|---------------------|------------------------------------------|
| `LangChain`         | Orchestrates loading, splitting, QA chain |
| `PyPDFLoader`       | Parses PDF pages                         |
| `RecursiveCharacterTextSplitter` | Breaks down large texts     |
| `HuggingFaceEmbeddings` | Generates vector embeddings         |
| `Chroma`            | Local vectorstore                        |
| `Ollama`            | Hosts the LLaMA 3.1 8B model locally     |

---

## 🚀 How to Use

1. **Set up Ollama** on your local machine:  
   Follow instructions at: [https://ollama.com](https://ollama.com)  
   Ensure the model `llama3:8b` is pulled using:
   ollama pull llama3:8b
   
2. **Open the notebook in Google Colab**

3. **Upload your PDF** when prompted

4. Ask questions directly in the cell input — type `"exit"` to stop

---

## 📦 Installation Requirements

This notebook assumes the following Python packages are available:

```bash
pip install langchain langchain-community langchain-huggingface langchain-chroma ollama tqdm
```

## 📄 Sample Usage

Ask a question (or 'exit'): What is the main topic of this document?
🧠 Answer: The main topic of the document is...

## 🧠 Credits

Built using:
- [LangChain](https://www.langchain.com/)
- [Ollama](https://ollama.com/)
- [Hugging Face Embeddings](https://huggingface.co/)
- [Chroma](https://www.trychroma.com/)
