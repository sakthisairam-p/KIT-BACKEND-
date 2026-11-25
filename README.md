# KIT-BACKEND-


```bash
1. Backend setup
cd backend
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python -m uvicorn app.main:app --reload --host 0.0.0.0 --port 8000

2. SYSTEM ARCHITECTURE(BACKEND)
rag-document-intelligence/
├── backend/
│   ├── app/
│   │   ├── __init__.py
│   │   ├── main.py
│   │   ├── config.py
│   │   ├── models/
│   │   │   └── schemas.py
│   │   ├── routes/
│   │   │   ├── chat.py
│   │   │   ├── dashboard.py
│   │   │   └── documents.py
│   │   └── services/
│   │       ├── document_processor.py
│   │       ├── embedding_service.py
│   │       ├── llm_service.py
│   │       ├── repository.py
│   │       ├── semantic_search.py
│   │       ├── text_chunker.py
│   │       └── vector_store.py
│   ├── chroma_db/
│   ├── data/
│   ├── uploads/
│   ├── requirements.txt
│   └── .env.example
