# NexaDocs AI

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

<div align="center">
  <h3>AI-Powered Document Analysis Platform with Advanced RAG Pipeline</h3>
  <p>
    <a href="https://github.com/hardikjain1704/NexaDocs-AI?tab=readme-ov-file#-core-features">Core Features</a> ·
    <a href="https://github.com/hardikjain1704/NexaDocs-AI?tab=readme-ov-file#%EF%B8%8F-architecture">Architecture</a> ·
    <a href="https://github.com/hardikjain1704/NexaDocs-AI?tab=readme-ov-file#-getting-started">Getting Started</a>
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
git clone https://github.com/hardikjain1704/NexaDocs-AI.git
cd NexaDocs-AI
python -m venv venv  
venv\Scripts\Activate
pip install -r requirements.txt
```

### Configuration
Required environment variables: (Refer .env.copy)
- GROQ_API_KEY
- GOOGLE_API_KEY

### Running
```bash
uvicorn api.main:app --reload
```

## 📁 Project Structure
```
NexaDocs-AI/
├── api/                       # API endpoints for serving document portal features
│   └── main.py
├── config/                    # App configuration files (YAML, constants, etc.)
│   └── config.yaml
├── data/                      # Uploaded and processed document storage (auto-generated, session-based)
│   └── [runtime generated, not in repo]
│                              # Data archival strategy: maintains a fixed max number of session folders;
│                              # oldest sessions are auto-deleted when the limit is exceeded.
├── exception/                 # Custom exception handling classes
│   ├── __init__.py
│   ├── custom_exception.py
│   └── custom_exception_archive.py
├── faiss_index/               # Stores FAISS vector indexes for sessions (auto-generated)
│   └── [runtime generated, not in repo]
├── logger/                    # Logging utilities and custom logger configuration
│   ├── __init__.py
│   └── custom_logger.py
├── logs/                      # Application logs (auto-generated)
│   └── [runtime generated, not in repo]
├── model/                     # Data models / ORM definitions
│   └── models.py
├── prompt/                    # Prompt templates for AI interactions
│   ├── __init__.py
│   └── prompt_library.py
├── src/                       # Core application modules
│   ├── document_analyzer/     # Logic for analyzing documents
│   │   ├── __init__.py
│   │   └── data_analysis.py
│   ├── document_chat/         # Retrieval-based chat over documents
│   │   ├── __init__.py
│   │   └── retrieval.py
│   ├── document_compare/      # Document comparison features
│   │   ├── __init__.py
│   │   └── document_comparator.py
│   ├── document_ingestion/    # Ingestion & preprocessing of documents
│   │   ├── __init__.py
│   │   └── data_ingestion.py
│   └── __init__.py
├── static/                    # Static assets (CSS, images)
│   └── style.css
├── templates/                 # HTML templates for UI
│   └── index.html
├── utils/                     # Helper utilities
│   ├── __init__.py
│   ├── config_loader.py       # Load and manage configs
│   ├── document_ops.py        # Document processing helpers
│   ├── file_io.py             # File read/write utilities
│   └── model_loader.py        # Model loading utilities
├── .env                       # Environment variables (not committed)
├── .env.copy                  # Example env file
├── .gitignore
├── main_archive.py            # Archived main script version
├── README.md
├── requirements.txt           # Python dependencies
├── setup.py                   # Package setup script
├── streamlit_ui.py            # Streamlit UI entry point
└── versions.py                # Version tracking
```

## 🛣️ Planned Features

- [ ] Query rewriting (RAG Fusion/ReAct)
- [ ] MMR reranking
- [ ] Local LLM integration
- [ ] Docker containerization
- [ ] AWS deployment architecture
- [ ] Additional document formats

## 📄 License
This project is licensed under the [MIT License](./LICENSE) © 2025 Hardik Jain.


## 📫 Contact
- Email: hardikjain1704@gmail.com
- LinkedIn: [Hardik Jain](https://www.linkedin.com/in/hardik-jain-8878a4290)


