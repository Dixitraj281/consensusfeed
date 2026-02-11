# ConsensusFeed 🚀  
### A Serverless, Multi-Agent AI System for High-Quality Tech & Research News Curation

ConsensusFeed is an **automated AI-powered news intelligence platform** that collects **1000+ AI and technology articles** every few hours and distills them into **25 high-quality, fact-checked, explainable news items** using a **multi-agent LLM consensus pipeline**.

The system runs **entirely serverlessly** using GitHub Actions for computation and GitHub Pages for delivery, achieving **near-zero infrastructure cost** with **infinite read scalability**.

---

## Problem Statement

AI and tech professionals face severe information overload:

- Thousands of repetitive, low-quality articles daily  
- No reliable signal for credibility, bias, or impact  
- Manual filtering wastes hours every week  
- Traditional aggregators rely on keywords and popularity, not intelligence  

The result is more noise than insight.

---

## Solution Overview

ConsensusFeed solves this using:

- **Multi-agent LLM filtering** instead of single-model judgment  
- **Explainable scoring** across relevance, novelty, credibility, and impact  
- **Consensus-based decision making** to reduce bias and hallucinations  
- **Fully serverless architecture** with no servers or databases  
- **Static JSON APIs** that scale infinitely via CDN  

The output is a **small, high-signal news set** that users can trust.

---

## System Architecture

30+ News Sources (RSS + APIs)
            ↓
Async Collection (Python)
            ↓
Stage 1: Bulk AI Filtering (Fast LLMs)
            ↓
Stage 2: Deep Intelligence (Fact, Bias, Credibility)
            ↓
Stage 3: Consensus Engine
            ↓
Static JSON APIs + AI Audio Digest
            ↓
GitHub Pages (CDN Cached)

---

## Core Features

- Multi-agent AI pipeline (Bulk → Deep → Consensus)
- Explainable article scoring across multiple dimensions
- Coverage of academic, industry, open-source, and government sources
- AI-generated audio news digest
- Fully automated CI/CD pipeline running every 4 hours
- Zero-infrastructure deployment
- Open and auditable decision logic

---

## Tech Stack and Design Rationale

Backend: Python 3.11  
LLMs: Groq API (LLaMA, Gemma)  
Frontend: Vanilla JavaScript + HTML  
Orchestration: GitHub Actions  
Hosting: GitHub Pages  
Data Storage: Static JSON  
Audio: Gemini TTS  

Design principle: **Maximum intelligence with minimum infrastructure**.

---

## Repository Structure

ConsensusFeed/
├── README.md
├── LICENSE
├── .gitignore
├── .env.example
├── src/
│   ├── backend/
│   ├── frontend/
│   └── shared/
├── .github/workflows/
└── scripts/

---

## Multi-Agent Consensus Pipeline

1. Bulk intelligence stage filters ~1000 articles to ~300  
2. Deep intelligence stage performs fact, bias, and credibility checks  
3. Consensus engine produces final 25 curated articles  

This design minimizes hallucinations and reduces single-model bias.

---

## Cost and Performance

- ~1000 articles processed per run  
- ~25 final curated articles  
- ~44 minutes per pipeline execution  
- ~$50–60 per month total cost  
- ~20× cheaper than traditional cloud architectures  

Static APIs ensure user traffic does not increase backend costs.

---

## Running Locally

git clone https://github.com/Dixitraj281/consensusfeed
cd consensusfeed  
python3 -m venv venv  
source venv/bin/activate  
pip install -r requirements.txt  
python src/backend/orchestrator.py  

---

## Deployment

- Fully automated via GitHub Actions  
- Executes every 4 hours  
- Generates updated JSON APIs and audio digest  
- Deploys automatically to GitHub Pages  

---

## Future Scope

- Personalized feeds per user  
- Real-time breaking news alerts  
- Newsletter and Slack integrations  
- Source reliability tracking  
- Topic clustering and trend prediction  
- Monetized API access  

---

## Author

Dixitraj  
Software Engineer | AI Systems | Distributed Pipelines
