# Medical RAG Chatbot

An AI-powered medical chatbot built using Retrieval-Augmented Generation (RAG) that provides accurate, context-aware answers from medical documents. The system is designed with a production-ready architecture, integrating vector search, LLM reasoning, and a fully automated CI/CD pipeline.

This project demonstrates how to build and deploy a secure, scalable AI application, combining LLMs with efficient retrieval systems and DevOps best practices.

---

## 📌 Project Overview

The Medical RAG Chatbot enables users to query medical documents and receive precise, context-based responses.

It handles:

- PDF document ingestion and processing
- Text embedding using transformer models
- Vector storage with FAISS
- Context retrieval for user queries
- LLM-based response generation
- Web-based chatbot interface
- Containerization and CI/CD deployment
- Security scanning before deployment

The system ensures that responses are grounded in real medical data, reducing hallucinations and improving reliability.

---

## How it works
The application follows a Retrieval-Augmented Generation (RAG) pipeline:

- Medical PDFs are loaded and processed
- Text is converted into embeddings
- Embeddings are stored in a FAISS vector database
- User queries are converted into embeddings
- Relevant documents are retrieved using similarity search
- Retrieved context is passed to the LLM
- The LLM generates a grounded response
- The chatbot interface displays the answer

This approach ensures responses are based on actual data rather than purely generative outputs.


### System Responsibilities

| Component          | Description                                  |
| ------------------ | -------------------------------------------- |
| PDF Loader         | Extracts and processes medical documents     |
| Embedding Model    | Converts text into vector representations    |
| FAISS Vector Store | Stores and retrieves embeddings efficiently  |
| Retriever          | Finds relevant context for user queries      |
| LLM                | Generates responses using retrieved context  |
| Flask App          | Serves the chatbot interface                 |
| CI/CD Pipeline     | Automates build, scan, and deployment        |
| Trivy Scanner      | Ensures container security before deployment |

---

##  Tech Stack

### AI & Backend
- LangChain - RAG pipeline orchestration
- FAISS - Vector database for similarity search
- HuggingFace - Embedding and LLM models
- Python
### Application Layer
- Flask
- HTML/CSS
### DevOps & Cloud Infrastructure
- Docker
- Jenkins
- Aqua Trivy - Security scanning
- AWS ECR - Container registry
- AWS Runner / EC2 - Deployment environment

## Core Design Decisions

- Retrieval-Augmented Generation
Ensures responses are grounded in real medical documents
- Vector database usage
FAISS enables fast and scalable similarity search
- Secure CI/CD pipeline
Trivy scans Docker images before deployment
- Modular architecture
Clear separation between data processing, retrieval, and generation
- Production-ready deployment
Automated pipeline using Jenkins and AWS infrastructure
---

## Getting Started


 **Local Development:**
   - Clone this repository.
   - Install dependencies from requirements.txt
   - Add your HuggingFace API key
   - Run the Flask application "python app.py"
---

## 🔄 Application Flow

1. User uploads or queries medical data
2. PDFs are processed and embedded
3. Embeddings are stored in FAISS
4. User enters a query in the chatbot
5. Retriever fetches relevant context
6. LLM generates response using context
7. Flask UI displays the answer

---

### CI/CD Deployment

The CI/CD pipeline is fully automated using Jenkins:

1. Code checkout from GitHub
2. Docker image build
3. Security scan using Trivy
4. Image pushed to AWS Elastic Container Registry
5. Deployment to AWS environment

Stage             | Tool Used
----------------- | ---------------------------------------
Build             | Jenkins
Containerization  | Docker
Security Scan     | Trivy
Image Registry    | AWS ECR
Deployment        | AWS EC2 / Runner

## ☁️ Deployment

- Jenkins handles CI/CD automation
- Docker containers are built and scanned
- Images are stored in AWS ECR
- Application deployed on AWS compute environment

---

## What This Project Demonstrates

- Retrieval-Augmented Generation (RAG) systems
- Vector search using FAISS
- LLM integration with real-world data
- Secure AI deployment with Trivy
- CI/CD automation using Jenkins
- Cloud deployment using AWS

---

## Future Improvements

- Add conversational memory
- Improve UI with modern frontend frameworks
- Integrate medical APIs for real-time data
- Deploy using Kubernetes for scalability
---

##  Author

**Tobi Segun Oluwategbe**  
AI & Cloud  
