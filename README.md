# 🧠 Beyond the Pages: Einstein & Bohr as Conversational Agents

This project brings Albert Einstein and Niels Bohr to life using **Retrieval-Augmented Generation (RAG)**. By grounding responses in their authentic writings and generating answers to curated questions, the system creates AI agents that mimic their reasoning and writing styles.

## 📁 Repository Structure

- `data/`
  - `einstein_cleaned_final.txt` — Einstein's cleaned writings
  - `bohr_cleaned_final.txt` — Bohr's cleaned writings
  - `einstein_300_questions.txt` — Questions for Einstein
  - `bohr_300_questions.txt` — Questions for Bohr

- `Model_Einstein.ipynb` — Generation pipeline for Einstein  
- `Model_Bohr.ipynb` — Generation pipeline for Bohr  
- `Model_classification.ipynb` — Classifier to detect style differences  
- `requirements.txt` — Python dependencies  
- `README.md` — This file

## 🧪 What This Project Does

- Embeds historical writings using Sentence-BERT
- Retrieves relevant content for each question
- Uses GPT-Neo (or similar) to generate persona-styled answers
- Evaluates stylistic fidelity with `StyleSim` and semantic relevance with `QuerySim`
- Tests distinguishability using a persona classifier

## 🚀 Getting Started

1. Install dependencies:
```bash
pip install -r requirements.txt```

> Note: Use `faiss-gpu` instead of `faiss-cpu` if you're on a GPU machine.

2. Run notebooks in order:
   - `Model_Einstein.ipynb` and `Model_Bohr.ipynb`
   - `Model_classification.ipynb`

## 📂 About the Data

All text corpora and questions are included under `data/`.

- `*_cleaned_final.txt`: Public domain excerpts cleaned for embedding
- `*_300_questions.txt`: Persona-aligned prompts to probe the model

> These writings are from public archives and are used strictly for educational and research purposes.

## 🧠 Acknowledgments

- Hugging Face Transformers & Sentence-Transformers  
- Facebook AI (for the original RAG framework)  
- Archive.org, Project Gutenberg (for historical text sourcing)



