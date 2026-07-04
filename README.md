# 🎓 College Placement RAG Chatbot (n8n)

An AI-powered Retrieval-Augmented Generation (RAG) chatbot built using **n8n**, **OpenAI**, **Supabase Vector Store**, and **Google Drive**. The workflow automatically ingests placement-related PDF documents, converts them into vector embeddings, and enables users to ask natural language questions about college placements.

## 🚀 Features

* Automated PDF ingestion from Google Drive
* Semantic search using OpenAI embeddings
* Vector storage with Supabase
* AI-powered question answering with GPT-4o Mini
* Low-code implementation using n8n
* Easy to customize for any document collection

## 🛠️ Tech Stack

* n8n
* OpenAI API (GPT-4o Mini & Embeddings)
* Supabase Vector Store
* Google Drive
* LangChain Nodes

## 📌 Workflow

1. Download placement PDF from Google Drive.
2. Load and extract document content.
3. Generate embeddings using OpenAI.
4. Store embeddings in Supabase Vector Store.
5. Accept user questions through the chat trigger.
6. Retrieve the most relevant document chunks.
7. Generate accurate answers using GPT-4o Mini.

## 📂 Project Structure

```text
workflow.json          # n8n workflow export
README.md              # Project documentation
screenshots/           # Workflow and chatbot screenshots
sample-data/           # Example documents (optional)
```

## 📷 Architecture

```
Google Drive PDF
        │
        ▼
Document Loader
        │
        ▼
OpenAI Embeddings
        │
        ▼
Supabase Vector Store
        │
        ▼
      AI Agent
        │
        ▼
   User Response
```

## ⚙️ Setup

1. Clone this repository.
2. Import `workflow.json` into your n8n instance.
3. Configure the following credentials:

   * OpenAI API
   * Google Drive OAuth
   * Supabase
4. Update the Google Drive file ID (or replace it with your own document).
5. Execute the indexing workflow once.
6. Open the chat interface and start asking questions.

## 💬 Example Questions

* What is the placement process?
* Which companies visited the campus?
* What is the average package offered?
* What are the eligibility criteria for placements?
* When do placements usually begin?

## 📖 Use Cases

* College placement information systems
* University document assistants
* Internal knowledge base chatbots
* HR and policy document search
* Educational RAG applications

## 🔮 Future Improvements

* Hybrid Retrieval (BM25 + Vector Search)
* Metadata filtering
* Multi-document support
* Reranking for improved accuracy
* Conversation memory
* Source citations in responses

## 👨‍💻 Author

**Dhruv Bhalla**

GitHub: https://github.com/dhruvbhalla14
