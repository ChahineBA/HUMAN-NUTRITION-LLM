# 🧠 RAG LLM for *Human Nutrition (2020)*

This repository contains a **Retrieval-Augmented Generation (RAG)** workflow built using *Human Nutrition (2020)* as the primary knowledge source. The project uses a combination of **document embedding**, **contextual search**, and a **Large Language Model (LLM)** to provide accurate and context-aware answers to nutrition-related queries. 🚀

## 🌟 Features
- 📄 **Document Preprocessing**: Converts large PDFs or textbooks into manageable chunks of text.
- 🧠 **Embeddings Creation**: Generates embeddings for the chunks using state-of-the-art models (e.g., `sentence-transformers`).
- 📚 **Contextual Search**: Retrieves the most relevant passages for a given query.
- 🤖 **LLM Integration**: Leverages an LLM to generate precise answers based on relevant context.
- 🖥️ **Local GPU Acceleration**: Designed to run efficiently on a local GPU, even for large datasets.
- 💬 **Optional Chat UI**: Provides an easy-to-use interface for interacting with the model.

---

## 📜 Workflow Overview

The following workflow illustrates the RAG pipeline implemented in this project:

![Workflow](simple-local-rag-workflow-flowchart.png)

1. **Document Preprocessing and Embedding Creation**
   - Load the source document (e.g., textbook or PDFs).
   - Split the document into smaller, context-friendly chunks (e.g., 10 sentences).
   - Generate embeddings for these chunks using models from Hugging Face or similar frameworks.
   - Store embeddings for fast retrieval or in a vector database (if dataset is large).

2. **Search and Answer**
   - Users submit a query (e.g., "What are macronutrients?").
   - The system retrieves the most relevant document chunks based on query similarity.
   - The LLM generates a detailed, context-aware response using the query and retrieved chunks.
   - Optionally, interact through a web-based chat interface.

---
## 🧪 Example Query

**Query**: *"What are macronutrients and their role in human health?"*

**Response**: *"Macronutrients are nutrients required in large amounts for energy and bodily functions. They include carbohydrates, proteins, and fats. Carbohydrates provide energy, proteins are essential for growth and repair, and fats play a crucial role in hormone production and cell structure."*

---

## 📊 Libraries Used

- `sentence-transformers` for embeddings.
- Hugging Face Transformers for the LLM.
- PyTorch for GPU acceleration.
- Optional: `gradio` or `streamlit` for the chat UI.

---

## 🎯 Future Work

- 🗄️ **Integrate a vector database** for scalability (e.g., FAISS or Pinecone).
- 🌐 **Deploy the system as a web app**.
- 🔄 **Expand to other domains or documents**.

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork this repository, submit issues, or open pull requests.

