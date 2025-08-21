# 🗺️ Detailed Roadmap

## Stage 1 — Foundations (this repo)
- [x] Prompting Basics notebook (zero vs few-shot)
- [x] CoT/ToT notebook with small example
- [x] Minimal RAG: chunk → embed → index (FAISS) → retrieve → answer

## Stage 2 — Make it rigorous
- [ ] Add a tiny evaluation harness:
  - [ ] Fixed test questions
  - [ ] Track prompt variants and outputs
  - [ ] Qualitative notes + basic retrieval stats (k, chunk size)
- [ ] Document reproducible experiments

## Stage 3 — Product polish
- [ ] Streamlit or Gradio UI for the RAG demo
- [ ] Deploy to Hugging Face Spaces
- [ ] Add screenshots/GIFs to README

## Stage 4 — Agents & n8n
- [ ] Build a workflow to watch a site (e.g., gov notifications)
- [ ] Summarize changes via RAG
- [ ] Daily/weekly email or Telegram alerts

## Nice-to-haves
- [ ] Add `pre-commit` hooks (black, isort)
- [ ] Add Dockerfile for fully reproducible env
- [ ] Add basic unit tests for utils