# 🤖 Smart AI Multi-Tool Assistant (Task 5)

This project is a **Streamlit-based AI assistant** that intelligently answers user queries by combining multiple tools, including internal knowledge retrieval, calculations, and general knowledge lookup.

---

## Features

- **Multi-Tool Query Handling**
  - **GlobalMart RAG System:** Uses **FAISS** + **SentenceTransformers** to retrieve answers from internal company documents.
  - **Calculator:** Safely evaluates arithmetic expressions.
  - **Wikipedia Search:** Fetches concise summaries from Wikipedia for general knowledge questions.

- **LLM Integration**
  - **Google Gemini API:** Automatically splits multi-part queries, selects appropriate tools, and synthesizes final answers.
  - **Query Routing:** Determines which tool to use for each part of a multi-part question.

- **Streamlit Frontend**
  - User-friendly interface with input box, buttons, and sidebar configuration.
  - Upload internal documents (TXT) or use sample demo documents.
  - Displays tool-wise outputs and a final synthesized answer.

- **Embeddings & Vector Search**
  - **SentenceTransformers (`all-MiniLM-L6-v2`)** for embedding document text.
  - **FAISS** for fast similarity search.

- **Advanced Features**
  - Handles multi-part queries separated by `AND` or `;`.
  - Combines outputs from different tools into a **concise final answer**.
  - Input validation and error handling for robust execution.

