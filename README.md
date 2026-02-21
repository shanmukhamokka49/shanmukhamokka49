# Hi, I'm Shanmukharao Mokka 👋

**Junior AI / ML Engineer** · LLMs · RAG Systems · Fine-Tuning · MLOps

[LinkedIn](https://linkedin.com/in/shanmukharaomokka7038) · [Email](mailto:mokkashanmukha78@gmail.com) · [Portfolio](https://shanmukharao.dev) · [HuggingFace](https://huggingface.co/shanmukharao-mokka) · [Kaggle](https://kaggle.com/shanmukharaomokka)

> 🟢 **Actively seeking AI/ML Internships & Entry-Level roles — Available immediately**
> 📍 Remote · Hybrid · US On-site | 📋 F-1 OPT · No immediate sponsorship needed

---

## About Me

CS graduate specializing in AI/ML with hands-on experience building production LLM
applications — RAG pipelines, fine-tuned open-source models, and autonomous AI agents.
I write clean Python, understand the math behind transformers, and know how to take a
model from prototype to a deployed API. I learn fast and I'm genuinely passionate about AI.

**B.S. Computer Science** — AI/ML Specialization | GPA: 3.8 / 4.0 | 2025

---

## Model Expertise

```
                     Proficiency                    Experience
──────────────────────────────────────────────────────────────────────────────
LLMs
  GPT-4o / GPT-3.5   ████████████████████░  95%    API · Tool Use · Agents
  LLaMA 3 8B/70B     ███████████████████░░  88%    LoRA Fine-Tune · Local Deploy
  Mistral 7B         ██████████████████░░░  85%    QLoRA · GGUF · vLLM
  Claude 3.5 Sonnet  ████████████████████░  92%    RAG · Long Context

Embeddings & Search
  text-embedding-3   ████████████████████░  95%    Semantic Search · Clustering
  BGE-M3 / E5-Large  ███████████████████░░  88%    Multilingual · Hybrid Search
  ColBERT / BM25     ███████████████░░░░░░  78%    Reranking · Sparse Retrieval

Vision & Audio
  CLIP / OpenCLIP    ██████████████████░░░  85%    Zero-shot · Image Search
  Whisper            ███████████████████░░  88%    ASR · Transcription Pipelines
  LLaVA              ████████████░░░░░░░░░  65%    VQA · Image Captioning
──────────────────────────────────────────────────────────────────────────────
```

---

## Architecture

**RAG Pipeline**
```
 User Query
     │
     ▼
 Query Rewrite (GPT-4o)  ──▶  Embed (BGE-M3)  ──▶  Vector DB (Pinecone + BM25)
                                                              │
                                                    Reranker (Cohere CE)
                                                              │
                                                      LLM (GPT-4o)  ──▶  Response
```

**LoRA Fine-Tuning Pipeline**
```
 Base Model (LLaMA 3 8B)
     │
     ├──▶  Freeze Weights
     │
     └──▶  Inject LoRA Adapters (r=16, α=32)
                    │
           Custom Dataset (Alpaca format)
                    │
           HF Trainer + bitsandbytes (4-bit NF4)
                    │
           ┌────────┴────────┐
           ▼                 ▼
      Merge + vLLM      GGUF → Ollama
```

**Transformer — How It Works**
```
 Token IDs  ──▶  Embeddings + Positional Encoding
                          │
              ┌───────────▼───────────┐
              │   Multi-Head Attention │   Attention(Q,K,V) = softmax(QKᵀ/√dₖ)·V
              └───────────┬───────────┘
                    Add & LayerNorm
              ┌───────────▼───────────┐
              │   Feed-Forward Net    │   FFN(x) = max(0, xW₁+b₁)W₂+b₂
              └───────────┬───────────┘
                    Add & LayerNorm
                          │
                    × N Layers  ──▶  Linear  ──▶  Softmax  ──▶  Token
```

---

## Projects

| Project | Description | Stack | Result |
|---------|-------------|-------|--------|
| **[DocuMind](https://github.com/shanmukharao-mokka/documind)** | RAG chatbot answering questions over 10K+ internal PDFs using hybrid search, Cohere reranking, and GPT-4o streaming | LangChain, GPT-4o, Pinecone, FastAPI, Docker | Sub-2s latency |
| **[LLaMA-3 Fine-Tuner](https://github.com/shanmukharao-mokka/llama3-finetuner)** | One-command QLoRA pipeline — raw dataset to quantized deployed model with full W&B experiment tracking | PyTorch, PEFT, bitsandbytes, W&B, Ollama | 4-bit, 8B params |
| **[MultiModal Search](https://github.com/shanmukharao-mokka/multimodal-search)** | Natural language → image retrieval over 1M+ images using CLIP embeddings and Qdrant vector DB | CLIP, Qdrant, FastAPI, Streamlit | < 100ms retrieval |
| **[AutoAgent](https://github.com/shanmukharao-mokka/autoagent)** | Autonomous LLM agent with tool calling, persistent memory, and multi-step planning for complex tasks | GPT-4o, OpenAI Functions, Redis, FastAPI | 5+ tool integrations |

---

## Tech Stack

**AI / ML** — Python, PyTorch, HuggingFace Transformers, LangChain, LangGraph, OpenAI API, scikit-learn, PEFT, bitsandbytes, NLTK, spaCy

**Vector & Search** — Pinecone, Qdrant, ChromaDB, FAISS, BM25, Cohere Rerank

**Infrastructure** — FastAPI, Docker, AWS (EC2, S3, Lambda), PostgreSQL, Redis, Git

**MLOps** — Weights & Biases, MLflow, GitHub Actions

**Models** — GPT-4o, LLaMA 3, Mistral 7B, Claude 3.5, Whisper, CLIP, BGE-M3, Sentence-BERT

---

## Certifications

| Credential | Issuer | Year |
|---|---|:---:|
| Deep Learning Specialization | DeepLearning.AI | 2024 |
| LLMs with Python & HuggingFace | DeepLearning.AI | 2024 |
| MLOps Specialization | DeepLearning.AI | 2024 |
| AWS Certified Cloud Practitioner | Amazon Web Services | 2023 |
| Applied Data Science with Python | University of Michigan | 2023 |
| LLM Science Exam — Top 15% | Kaggle | 2023 |

---

## Currently Learning

| Status | Topic |
|:---:|---|
| ✅ | QLoRA · DPO Fine-Tuning · LangGraph · Pinecone · Qdrant |
| 🔄 | OpenAI Realtime API · Multimodal Models · Voice Agents |
| 📅 | CUDA Kernels · RLHF · AWS SageMaker · TensorRT |

---

## Open to Opportunities

I'm looking for an AI/ML internship or entry-level role where I can contribute to real
AI products from day one  not just run experiments, but help ship things. I ramp up
fast and I'm at my best solving problems that haven't been solved before.

**Target roles:** AI/ML Intern · ML Engineer (New Grad) · LLM/NLP Engineer · Data Science Intern

📬 [mokkashanmukha78@gmail.com](mailto:mokkashanmukha78@gmail.com)
🔗 [linkedin.com/in/shanmukharaomokka7038](https://linkedin.com/in/shanmukharaomokka7038)
🌐 [shanmukharao.dev](https://shanmukharao.dev)

---
