# 🧠 AI Medical Assistant (RAG + AWS Bedrock)

An AI-powered medical assistant that allows users to upload medical documents (PDFs) and ask questions. The system uses Retrieval-Augmented Generation (RAG) with AWS Bedrock (LLaMA 3 + Titan Embeddings) to provide accurate answers.

---

## 🚀 Features

- 📄 Upload medical PDFs
- 🤖 Ask questions based on uploaded documents
- 🧠 Uses AWS Bedrock (LLaMA 3)
- 🔎 FAISS vector database for semantic search
- 📊 Returns answers with source references

---

## 🏗️ Tech Stack

- **Backend:** FastAPI
- **Frontend:** Streamlit
- **LLM:** AWS Bedrock (Meta LLaMA 3)
- **Embeddings:** Amazon Titan
- **Vector DB:** FAISS
- **Language:** Python

---

## 📁 Project Structure

AI_Medical_Assistance/
│
├── backend/
│   ├── app/
│   ├── data/
│   ├── db/
│   └── requirements.txt
│
├── frontend/
│   └── app.py
│
└── README.md

---

## ⚙️ Setup Instructions

### 1. Clone repo

git clone https://github.com/subhakarRPeddakkagar/AI_Medical_Assistance.git
cd AI_Medical_Assistance

---

### 2. Backend setup

cd backend  
pip install -r requirements.txt  
uvicorn app.main:app --reload  

---

### 3. Frontend setup

cd frontend  
streamlit run app.py  

---

## 🔐 Environment Variables

Create `.env` inside backend:

AWS_ACCESS_KEY_ID=your_key  
AWS_SECRET_ACCESS_KEY=your_secret  
AWS_REGION=us-east-1  

BEDROCK_MODEL_ID=meta.llama3-8b-instruct-v1:0  
EMBEDDING_MODEL_ID=amazon.titan-embed-text-v1  

---

## 📌 API Endpoints

- POST /upload → Upload PDF  
- POST /ask → Ask questions  

---

## ⚠️ Disclaimer

This application is for educational purposes only and should not replace professional medical advice.

---

## 👨‍💻 Author

Subhakar R Peddakagar
