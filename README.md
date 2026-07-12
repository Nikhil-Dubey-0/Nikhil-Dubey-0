<p align="center">
  <img src="./assets/header.svg" width="100%" alt="Nikhil Dubey — AI/ML Engineer. Retrieval systems, multi-agent orchestration, LLM evaluation."/>
</p>

<p align="center">
  <a href="https://linkedin.com/in/dubey-nikhil" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:nikhildubey2thousand3@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <a href="https://github.com/Nikhil-Dubey-0" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
</p>

---

## About

I build LLM systems that are held to account — where the numbers come from deterministic code and
the model is only allowed to interpret them, where every claim is checked before it's shown, and
where retrieval quality is measured rather than assumed.

Most of my work lives at the intersection of **retrieval** (hybrid search, reranking, evaluation)
and **agentic pipelines** (LangGraph, human-in-the-loop routing, grounding validators). I prefer
building the primitives myself before reaching for a framework — my RAG stack was written from
scratch, without LangChain, so I'd actually understand what the abstractions hide.

---

## Featured Work

### 🎼 [Orchestra](https://github.com/Nikhil-Dubey-0/Orchestra) — Multi-Agent Data Analysis Platform

<p>
  <img src="https://img.shields.io/badge/LangGraph-0D1117?style=flat-square&logo=langchain&logoColor=6C63FF"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
</p>

Upload a dataset and a team of specialized agents — orchestrated with **LangGraph** — profiles it,
proposes a cleaning plan for your approval, computes statistics, generates business insights,
validates every claim against the data, draws charts, and writes a downloadable report.

> **The core idea:** Python computes every number; the LLM only interprets. Each insight must cite
> a verified `fact_id`, and a deterministic validator re-checks it against the source statistic.
> Ungrounded claims are dropped — never shown as fact.

- **Human-in-the-loop interrupt** — the graph pauses for you to approve the cleaning plan, then resumes.
- **Conditional validation loop** — insights are regenerated if too many fail grounding; the UI surfaces a groundedness score.
- **Swappable LLM provider** — Groq, Gemini, Ollama, OpenAI, or Claude behind one env var, with per-node token and cost tracking.
- **FastAPI + SSE** streams the run live to a React/Vite agent monitor; **40 tests** pass with no API key and no network.

📖 [Architecture & docs](https://github.com/Nikhil-Dubey-0/Orchestra/tree/main/docs)

<br/>

### 🔍 [ContexFlow](https://github.com/Nikhil-Dubey-0/ContexFlow) — RAG, Built From Scratch

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logo=meta&logoColor=white"/>
  <img src="https://img.shields.io/badge/BM25-8B5CF6?style=flat-square"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
</p>

A Retrieval-Augmented Generation system written in pure Python — **no LangChain, no abstractions**.
Upload PDFs or DOCX, ask questions, get answers with exact page-level citations.

- **Hybrid retrieval** — FAISS (semantic) + BM25 (keyword) merged with Reciprocal Rank Fusion, lifting recall@5 from 0% to 50% over semantic-only search.
- **Cross-encoder reranking** and **LLM query rewriting** for relevance, at ~14ms retrieval latency across 622 chunks.
- **Token-by-token streaming** via Groq (Llama-3.3 70B), with chat history so follow-ups keep context.
- **Dual interface** — Streamlit chat UI and a FastAPI REST backend with auto-generated Swagger docs.

---

## Also On The Shelf

| Project | Description |
|---|---|
| 🚗 [**Traffic Monitoring System**](https://github.com/Nikhil-Dubey-0/Traffic-Monitoring-System) | Real-time vehicle detection with **YOLOv8** + OpenCV — motion tracking for speed estimation, rule-based congestion classification, and a Streamlit analytics dashboard. |
| 🎬 [**Movie Recommender**](https://github.com/Nikhil-Dubey-0/movie_app) | Content-based recommender over **5,000+ movies** using TF-IDF vectorization and cosine similarity, blended with popularity signals. |

---

## Tech Stack

<b>LLMs, Agents & Retrieval</b>
<p>
  <img src="https://img.shields.io/badge/LangGraph-0D1117?style=flat-square&logo=langchain&logoColor=6C63FF"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/RAG-6C63FF?style=flat-square"/>
  <img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logo=meta&logoColor=white"/>
  <img src="https://img.shields.io/badge/BM25-8B5CF6?style=flat-square"/>
  <img src="https://img.shields.io/badge/Transformers-FFD43B?style=flat-square&logo=huggingface&logoColor=black"/>
  <img src="https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white"/>
  <img src="https://img.shields.io/badge/Groq-F55036?style=flat-square&logo=groq&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white"/>
</p>

<b>Languages</b>
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white"/>
</p>

<b>ML / Deep Learning</b>
<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white"/>
  <img src="https://img.shields.io/badge/YOLOv8-111111?style=flat-square&logo=yolo&logoColor=00FFFF"/>
  <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black"/>
</p>

<b>Backend & Data</b>
<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white"/>
</p>

<b>Tooling</b>
<p>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visual-studio-code&logoColor=white"/>
</p>

---

## Currently Interested In

- **Grounding & verification** — forcing LLM output to cite deterministic computation, and building validators that reject what can't be traced back to the data.
- **Multi-agent orchestration** — human-in-the-loop interrupts, conditional routing, and state that survives a restart. Graphs, not scripts.
- **Retrieval quality** — hybrid search, reranking strategies, and actually measuring recall instead of trusting vibes.
- **LLM evaluation & safety** — prompt risk classification, response screening, and audit trails for AI systems that ship.
