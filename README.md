# FSTT Local AI Assistant - Ollama Lab

**Student Name:** Hachem Abdessamad
**Course:** 🤖 Mini-RAG & Local AI with Ollama Laboratory
**Date:** 26/10/2026

## Project Overview
This repository contains the complete practical lab on running and developing Local AI applications using Ollama and Python. The final deliverable is a fully local RAG (Retrieval-Augmented Generation) web application using Flask.

## Repository Structure
- `Local_AI_Ollama_Lab.ipynb`: The complete Jupyter Notebook with all exercises and answers.
- `report.pdf`: The final compiled LaTeX report (Q1 to Q15).
- `source/`: Python scripts (`app.py`, `rag.py`, `chatbot.py`, `benchmark.py`).
- `documents/`: The text files used as local knowledge for the RAG.
- `screenshots/`: Visual proof of the installation, models, chatbot, RAG, and webapp.

## How to run this project locally
1. Install [Ollama](https://ollama.com/download).
2. Pull the models:
   ```bash
   ollama pull qwen2.5:7b
   ollama pull gemma2:2b
   
# FSTT Local AI Assistant

A fully local assistant: Flask web UI → Ollama → local LLM, with a keyword (TF-IDF) retriever over `documents/`,
conversation history, structured (JSON) answers and response-time display.

## Setup
```bash
ollama pull qwen3.5
pip install flask requests psutil pandas
```

## Run
```bash
cd source
python app.py            # http://127.0.0.1:5001
python chatbot.py        # console chatbot
python benchmark.py qwen3.5 gemma3
```
Environment variables: `MODEL`, `OLLAMA_URL`, `PORT`.
