# 🧠 Beyond the Pages: Einstein & Bohr as Conversational Agents

This project brings Albert Einstein and Niels Bohr to life using **Retrieval-Augmented Generation (RAG)**. By grounding responses in their authentic writings and generating answers to curated questions, the system creates AI agents that mimic their reasoning and writing styles.

## 📁 Repository Structure

- `data/`
  - `einstein_cleaned_final.txt` — Einstein's cleaned writings
  - `bohr_cleaned_final.txt` — Bohr's cleaned writings
  - `einstein_300_questions.txt` — Questions for Einstein
  - `bohr_300_questions.txt` — Questions for Bohr

- `loading_and_preprocessing.ipynb` — Chunking, embedding, retrieval setup  
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


