# RAG-Project

This project demonstrates a simple yet complete RAG (Retrieval-Augmented Generation) pipeline built using LangChain, OpenAI, and Chroma for vector storage. The pipeline scrapes a GenAI course page, processes the content, converts it to vector embeddings, and uses an LLM to answer natural language questions grounded in that context.

## 🚀 Features

🔑 Secure API Key Retrieval via Google Colab userdata
🌐 Web Scraping from a live GenAI course page using WebBaseLoader
✂️ Document Chunking using RecursiveCharacterTextSplitter
🧠 Embeddings & Vector DB with OpenAI and ChromaDB
🔄 Retriever Setup for semantic search over the course content
💬 RAG Chain using LangChain's hub, ChatOpenAI, and output parsers
🧪 Test Queries for answering course-related questions

## 🧱 Tech Stack

LangChain (langchain, langchain-community, langchain-openai, langchainhub)
OpenAI Embeddings & ChatCompletion
Chroma for vector database
Python (Colab-friendly)

## 📦 Installation
!pip install langchain_community langchainhub chromadb langchain langchain-openai

## RAG Pipeline Flow

Web Scraping → WebBaseLoader
Text Chunking → RecursiveCharacterTextSplitter
Embeddings → OpenAIEmbeddings
Vector Store → Chroma.from_documents()
Retriever → .as_retriever()
Prompt Augmentation → hub.pull("rlm/rag-prompt")
LLM Invocation → ChatOpenAI
Response Parsing → StrOutputParser


