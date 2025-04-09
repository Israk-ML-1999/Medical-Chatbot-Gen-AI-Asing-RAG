# Medical-Chatbot-Gen-AI-Asing-RAG

🤖 A Medical Chatbot built using Groq's LLaMA 3 model, LangChain, and Pinecone vector database. Capable of answering medical queries from a PDF knowledge base. Powered by open-source LLMs with real-time, context-aware responses.

# 🩺 Medical Chatbot using Groq + LangChain + LLaMA 3 + Pinecone

A powerful and intelligent medical chatbot built using cutting-edge technologies like **Groq**, **LangChain**, **LLaMA 3**, and **Pinecone**. This chatbot can process and answer medical questions based on a given medical knowledge base in PDF format.

---

## 🚀 Features

- 🔍 **RAG (Retrieval-Augmented Generation)**: Searches context from a medical PDF file.
- 🧠 **LLaMA 3 via Groq API**: Fast and accurate open-source LLM responses.
- 🧱 **LangChain**: Manages document loading, embeddings, and QA chain.
- 🗂️ **Pinecone**: Efficient vector storage and retrieval.
- 📄 **PDF Support**: Upload any medical PDF as your knowledge base.
- 🛡️ **Secure API handling** via `.env`.
-  Flask-based Medical Chatbot app with a beautiful HTML + CSS frontend.

 # How it Works
1. Loads medical content from medical_knowledge.pdf.
2. Splits it into chunks and generates embeddings.
3. Stores embeddings in Pinecone.
4. On user query, fetches relevant chunks.
5. Passes context to LLaMA 3 via Groq API.
6. Returns context-aware response.


#Demo

![Image](https://github.com/user-attachments/assets/3cb46117-5825-4d8b-930b-af7468ef63e0)

![Image](https://github.com/user-attachments/assets/3cb76a7f-6e83-4e02-b93c-e2aa63be2138)

# How to run?
### STEPS:

Clone the repository

### Create a conda environment after opening the repository

```bash
conda create -n medibot python=3.10 -y
```

```bash
conda activate medibot
```


###  install the requirements
```bash
pip install -r requirements.txt
```


### Create a `.env` file in the root directory and add your Pinecone & openai credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
GROQ_API_KEY= xxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```


```bash
# run the following command to store embeddings to pinecone
python store_index.py
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up localhost:


