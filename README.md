# CodeMentor LLM — AI Coding Tutor with Repository Understanding

**CodeMentor LLM** is an AI-powered coding assistant designed to help developers understand, debug, analyze, and improve their codebases. Unlike traditional AI coding assistants that primarily work with isolated code snippets, CodeMentor aims to understand the structure and relationships within an entire GitHub repository.

By combining Large Language Models (LLMs), Retrieval-Augmented Generation (RAG), code analysis, and semantic search, the platform aims to provide context-aware programming assistance and personalized coding guidance.

## 🎯 Project Objective

The main objective of CodeMentor LLM is to make software development and programming concepts easier to understand by allowing users to interact with their own code repositories using natural language.

Users will be able to ask questions about their projects, understand complex functions, identify potential errors, and receive explanations based on their actual source code.

## ✨ Planned Features

### 1. Repository Understanding
- Connect and analyze GitHub repositories.
- Understand project folder and file structures.
- Identify programming languages, functions, and classes.
- Retrieve relevant code from different files.

### 2. AI Code Explainer
- Explain code in simple language.
- Provide line-by-line explanations.
- Understand complex functions and algorithms.
- Explain relationships between different components.

### 3. AI Debugging Assistant
- Analyze programming errors and exceptions.
- Identify potentially problematic code.
- Suggest possible solutions.
- Explain why an error occurs.

### 4. Repository-Aware AI Chat
- Ask natural-language questions about an entire codebase.
- Retrieve relevant code using semantic search.
- Generate context-aware answers.
- Provide relevant file references.

### 5. AI Code Review
- Identify potential logical errors.
- Suggest code improvements.
- Detect code duplication.
- Recommend better coding practices.

### 6. Project Viva Mode
- Generate technical questions based on the repository.
- Prepare project-specific viva questions.
- Evaluate user responses.
- Help students understand their project implementation.

### 7. Additional Planned Features
- AI-powered documentation generation.
- Code complexity analysis.
- Project architecture visualization.
- Git commit and code change explanation.
- Personalized programming assistance.

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Frontend | React.js, Vite |
| Styling | Tailwind CSS |
| Backend | Python, FastAPI |
| AI Model | Gemini API |
| Embeddings | Sentence Transformers |
| RAG | Retrieval-Augmented Generation |
| Vector Database | ChromaDB |
| Repository Integration | GitHub API |
| Code Parsing | Tree-sitter (planned) |

## 🧠 How It Works

CodeMentor LLM is designed around a repository-aware RAG pipeline.

1. **Repository Import:** Users connect a GitHub repository or upload a project.
2. **Code Extraction:** The backend extracts supported source files and analyzes the project structure.
3. **Code Chunking:** Source code is divided into meaningful sections.
4. **Embedding Generation:** Embeddings are generated to represent code sections numerically.
5. **Vector Storage:** Code embeddings and metadata are stored in ChromaDB.
6. **Semantic Retrieval:** Relevant code sections are retrieved based on the user's question.
7. **LLM Processing:** The retrieved context is provided to the LLM to generate relevant explanations.
8. **Response Generation:** The user receives repository-aware answers and coding assistance.

## 📂 Project Structure

```text
CodeMentor-LLM/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── dashboard/
│   │   └── chat/
│   └── package.json
│
├── backend/
│   ├── routes/
│   ├── services/
│   ├── database/
│   ├── utils/
│   ├── main.py
│   └── requirements.txt
│
├── .gitignore
└── README.md
```

*The structure will evolve as development progresses.*

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- Node.js and npm
- Git
- Gemini API key

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/CodeMentor-LLM.git
cd CodeMentor-LLM
```

### 2. Set Up the Backend

```bash
cd backend

python -m venv venv
```

Activate the virtual environment:

**Windows:**
```powershell
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### 3. Configure Environment Variables

Create a `.env` file inside the backend directory:

```env
GEMINI_API_KEY=your_api_key_here
```

Never upload API keys or sensitive credentials to GitHub.

### 4. Run the Backend

```bash
uvicorn main:app --reload
```

### 5. Set Up the Frontend

Open another terminal:

```bash
cd frontend
npm install
npm run dev
```

The frontend and backend setup instructions will be updated as the application develops.

## 🔮 Future Scope

- Support for multiple programming languages.
- Private GitHub repository integration.
- More advanced repository-level code understanding.
- AI-powered test case generation.
- Interactive code architecture visualization.
- Personalized learning and progress tracking.
- Improved code retrieval and evaluation.

## 🎓 Project Motivation

Understanding an existing codebase can be challenging, especially for students and beginner developers working with large projects.

CodeMentor LLM aims to bridge this gap by combining AI-powered code understanding with personalized programming education, making it easier to learn, debug, and work with real-world software projects.

---

**Project Status:** 🚧 Under Development

**Category:** Generative AI | Large Language Models | Software Development | RAG
