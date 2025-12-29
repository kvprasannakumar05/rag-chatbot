# RAG Chatbot - Ask Questions About Your Documents

A smart chatbot application that answers questions based on your own documents using **Retrieval-Augmented Generation (RAG)**. Instead of generic AI responses, this system retrieves relevant information from your documents and uses it to provide accurate, document-specific answers.

## 🎯 What This Project Does

- **Upload PDFs** → System processes and stores them in a vector database
- **Ask Questions** → Chat interface lets you query your documents
- **Get Smart Answers** → AI retrieves relevant info and answers based on YOUR data

## 🛠 Tech Stack

- **LangChain** - LLM orchestration and document processing
- **Pinecone** - Vector database for semantic search
- **OpenAI** - GPT models for intelligent responses
- **Streamlit** - Interactive web interface

## 📋 Prerequisites

- Python 3.11+
- Pinecone account (free tier available)
- OpenAI API key

## 🚀 Quick Start

### 1. Clone & Setup
```
https://github.com/kvprasannakumar05/rag-chatbot.git
```

### 2. Create Virtual Environment
```
python -m venv venv
venv\Scripts\Activate
```
*(On Mac): `source venv/bin/activate`*

### 3. Install Dependencies
```
pip install -r requirements.txt
```

### 4. Configure API Keys
1. Create free accounts:
   - [Pinecone](https://www.pinecone.io/)
   - [OpenAI API](https://platform.openai.com/api-keys)

2. Add keys to `.env` file:
   - Rename `.env.example` to `.env`
   - Add your Pinecone and OpenAI API keys

### 5. Run the Application
```
streamlit run chatbot_rag.py
```

The app will open at `http://localhost:8501`

## 📁 Project Structure

| File | Purpose |
|------|---------|
| `ingestion.py` | Processes PDFs and loads them into Pinecone |
| `retrieval.py` | Searches Pinecone for relevant documents |
| `chatbot_rag.py` | Interactive Streamlit chat interface |

## 💡 How It Works

1. **Document Ingestion** - PDFs are converted to text chunks and stored as embeddings
2. **Semantic Search** - User queries are matched against document chunks
3. **AI Response** - Retrieved documents + query sent to OpenAI GPT
4. **User Interface** - Streamlit displays the conversation

## 🎓 Key Skills Demonstrated

✅ Vector databases & embeddings  
✅ LLM integration & prompt engineering  
✅ Document processing pipelines  
✅ Full-stack application development  

---

