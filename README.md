# 🤖 Saibot – Resume-Aware Chatbot

Saibot is a Retrieval-Augmented Generation (RAG) based personal chatbot that answers questions specifically related to my resume. It uses a LLM and a vector store to ground its responses in my experience, skills, and background.

 🔗To know about me in detail: [https://soluchann.github.io/Saibot](https://soluchann.github.io/Saibot)

---

## 🚀 Features

- Resume-aware Q&A chatbot
- RAG pipeline for grounding responses in my actual CV
- Simple UI for chatting
- Private

---

## 🧠 How It Works

- resume is split into chunks and embedded using a sentence transformer  
- Embeddings are stored in a vector database (neo4j)  
- When you ask a question, the chatbot:
  - Converts the query to a vector  
  - Retrieves the most relevant chunks from my resume  
  - Feeds both the query and the retrieved context to the LLM  
  - The LLM responds based only on my actual resume data

---
