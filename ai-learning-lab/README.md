# 🧠 AI Learning Lab
Hands-on experiments while I learn emerging AI concepts: **Prompt Engineering**, **Chain-of-Thought / Tree-of-Thought**, and **Retrieval-Augmented Generation (RAG)**.

> 🎯 Goal: Learn by building. Each folder contains runnable notebooks, clear explanations, and small milestones so I can demonstrate progress in public.

---

## 🔎 What’s inside
- `prompting-basics/` — Zero-shot vs few-shot prompting, prompt patterns, and evaluation.
- `cot-tot/` — Chain-of-Thought (CoT) and a tiny Tree-of-Thought (ToT) exploration.
- `rag-demo/` — Minimal RAG pipeline (chunking → embeddings → vector search → answer), with a simple UI option later.

---

## 🚀 Quickstart
1) **Clone & set up**
```bash
git clone https://github.com/<your-username>/ai-learning-lab.git
cd ai-learning-lab

# (Recommended) Create a virtual environment
python -m venv .venv && source .venv/bin/activate  # Windows: .venv\Scripts\activate

pip install -r requirements.txt
```

2) **Set your API keys (optional, for LLM responses)**  
Copy `.env.example` → `.env` and fill your values:
```
OPENAI_API_KEY=your_key_here
```

3) **Run notebooks**
```bash
python -m ipykernel install --user --name ai-learning-lab
jupyter lab  # or jupyter notebook
```

Open the notebooks in each folder and run top to bottom.

---

## 📚 Project Structure
```
ai-learning-lab/
│── README.md
│── ROADMAP.md
│── requirements.txt
│── .gitignore
│── .env.example
│
├── prompting-basics/
│   └── zero_vs_few_shot.ipynb
│
├── cot-tot/
│   └── reasoning_methods.ipynb
│
└── rag-demo/
    ├── minimal_rag.ipynb
    └── sample_data/
        ├── rag_note_1.txt
        └── rag_note_2.txt
```

---

## 🧩 Notebooks Overview
### 1) Prompting Basics
- Compare **zero-shot** vs **few-shot** on the same task.
- Try prompt patterns: role prompting, format constraints, and style guides.
- Keep results **side-by-side** and write short observations.

### 2) CoT & ToT
- Show a normal answer vs **CoT** (“think step-by-step”).
- Tiny **ToT** experiment: explore multiple reasoning branches and pick a best one.

### 3) RAG Demo
- Parse text files, **chunk**, compute **embeddings**, index with **FAISS**, and **retrieve** top-k chunks.
- Compose a final answer with retrieved context.
- Works without an API key (prints retrieved context), or uses an LLM if you configure `OPENAI_API_KEY`.

---

## ✅ How to Show Progress on GitHub
- Use clear commit messages:
  - `feat(prompting): add zero vs few-shot comparison`
  - `chore(rag): add sample_data and chunker util`
- Add screenshots/GIFs of notebook outputs in the README (drag & drop into GitHub issues to get image URLs).

---

## 🗺️ Roadmap (high-level)
- ✅ Stage 1: Minimal notebooks for prompting, CoT/ToT, and RAG
- ⬜ Stage 2: Add evaluation (simple metrics + qualitative notes)
- ⬜ Stage 3: RAG UI with Streamlit/Gradio (+ deployment)
- ⬜ Stage 4: Agents & n8n workflows (alerts, scheduled crawls)

See **ROADMAP.md** for details and tasks.

---

## ⚙️ Requirements
See `requirements.txt`. Notebooks try to install missing libs where possible.

> ℹ️ If you don’t have API keys, you can still run everything. The RAG notebook will print retrieved context and a template answer without LLMs.

---

## 📝 License
MIT — feel free to fork, learn, and build on top.