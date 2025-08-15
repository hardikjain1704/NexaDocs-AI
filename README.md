# NexaDocs AI

<div align="center">
  <h3>AI-Powered Document Analysis Platform with Advanced RAG Pipeline</h3>
  <p>
    <a href="#features">Features</a> ·
    <a href="#architecture">Architecture</a> ·
    <a href="#getting-started">Getting Started</a>
  </p>
</div>

## 🎯 Core Features

### Document Analysis
- **Single-Document Analysis**: Semantic question-answering with document context
- **Two-Document Comparison**: Side-by-side difference detection
- **Multi-Document Search**: Conversational search across documents
- **Session Memory**: Context-aware conversations with document history

### Technical Implementation
- **Document Processing**: 
  - PDF text extraction using PyMuPDF
  - Metadata enrichment (title, page number, source ID)
- **Vector Operations**:
  - FAISS/Chroma vector stores
  - Hugging Face and OpenAI embeddings
- **RAG Pipeline**:
  - LangChain integration
  - Context-aware retrieval

## 🏗️ Architecture

### Backend
- FastAPI REST API
- Document processing service
- Vector database integration
- Session management

### Frontend
- HTML, CSS, JavaScript UI
- Document upload interface
- Interactive chat
- Comparison view

## 💻 Tech Stack
- **Backend**: FastAPI, LangChain
- **AI/ML**: OpenAI, Hugging Face
- **Vector Store**: FAISS, Chroma
- **Document Processing**: PyMuPDF
- **Frontend**: HTML, CSS, JavaScript

## 🚀 Getting Started

### Prerequisites
```bash
Python 3.10+
```

### Installation
```bash
git clone https://github.com/yourusername/document_portal.git
cd document_portal
pip install -r requirements.txt
```

### Configuration
Required environment variables:
- OPENAI_API_KEY
- HUGGINGFACE_API_KEY

### Running
```bash
uvicorn main:app --reload
```

## 📁 Project Structure
```
document_portal/
├── api/            # FastAPI routes
├── core/           # RAG implementation
├── static/         # Frontend assets
└── templates/      # HTML templates
```

## 🛣️ Planned Features

- [ ] Query rewriting (RAG Fusion/ReAct)
- [ ] MMR reranking
- [ ] Local LLM integration
- [ ] Docker containerization
- [ ] AWS deployment architecture
- [ ] Additional document formats

## 📄 License
MIT © [Hardik Jain]

## 📫 Contact
- Email: hardikjain1704@gmail.com
- LinkedIn: [Hardik Jain](https://www.linkedin.com/in/hardik-jain-8878a4290)


