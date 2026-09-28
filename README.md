## DocuMind — Intelligent Document Retrieval using RAG

DocuMind is a Retrieval-Augmented Generation (RAG) based system that enables users to upload documents and query them using natural language. The system processes documents through text extraction, preprocessing, chunking, and embedding, and stores them in a per-user FAISS vector index for efficient semantic search.

It implements controlled retrieval with top-k selection, similarity thresholding, and context filtering to minimize hallucinations. 

### Key Features
- Secure document upload with edge-case handling
- Text preprocessing, chunking, and metadata mapping
- Per-user FAISS indexing with incremental updates
- Semantic search with similarity thresholding
- Context-aware LLM responses with prompt control
- Query logging and system monitoring

### Tech Stack
- Backend: Django
- Vector DB: FAISS
- ML: Scikit-learn (Logistic Regression)
- LLM Integration: API-based
- Database: SQLite

### Pipeline
Upload → Preprocess → Chunk → Embed → Store (FAISS) -> Query → Embed → Filter + Retrieve → LLM → Answer
