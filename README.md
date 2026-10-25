HealthSync AI - End-to-End Medical Chatbot
Python Flask Docker LangChain License

An AI-powered medical assistant chatbot using Retrieval Augmented Generation (RAG) with LangChain, Groq, and Pinecone.

Overview
HealthSync AI is an intelligent medical chatbot that provides accurate health information and answers medical queries using advanced AI technologies. Built with Retrieval Augmented Generation (RAG), it combines the power of:

Large Language Models (LLM) via Groq API
Vector Database for medical knowledge retrieval (Pinecone)
Semantic Search using Sentence Transformers
Conversational Memory for context-aware responses
The chatbot can answer questions about symptoms, diseases, treatments, and general health information while maintaining conversation context.

Architecture
Architecture

Flow:

User sends a medical query through the web interface
Flask backend receives the query
Query is converted to embeddings using Sentence Transformers
Similar medical documents are retrieved from Pinecone vector store
Context + Query sent to Groq LLM (Llama 3.3 70B)
AI generates a contextually relevant response
Response sent back to user with conversation memory
Tech Stack
Backend
Framework: Flask 3.1.2
Server: Gunicorn 23.0.0
Language: Python 3.10
AI/ML
LLM: Groq API (Llama 3.3 70B Versatile)
Embeddings: Sentence Transformers (all-MiniLM-L6-v2)
Vector Database: Pinecone
Framework: LangChain 0.1.20
Frontend
HTML
CSS
JavaScript
Deployment
Containerization: Docker
Image Size: 13.81 GB
Base Image: Python 3.10-slim
Installation
Prerequisites
Python 3.10+
pip
Virtual environment (recommended)
Groq API Key
Pinecone API Key
1. Clone Repository
git clone https://github.com/arunkumareswari/End-to-End-Medical-Chatbot-Generative-AI.git
cd End-to-End-Medical-Chatbot-Generative-AI
2. Create Virtual Environment
python -m venv healthSync
healthSync\Scripts\activate
3. Install Dependencies
pip install -r requirements.txt
4. Environment Variables
Create a .env file in the root directory:

PINECONE_API_KEY=your_pinecone_api_key_here
GROQ_API_KEY=your_groq_api_key_here
Get API Keys:

Pinecone: https://app.pinecone.io/
Groq: https://console.groq.com/
5. Run Application
python app.py
Visit: http://localhost:8080

Screenshots
Chat Interface
Chat Interface

