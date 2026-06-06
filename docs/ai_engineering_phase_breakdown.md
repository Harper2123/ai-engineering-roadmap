# AI Engineering Mastery Roadmap

This roadmap is designed for a slow, consistent, project-driven path to mastering AI Engineering. It assumes:

- You will learn mainly through **books and projects**.
- You are **not in a hurry**.
- You already have a good job, so the goal is **long-term skill depth**, not short-term job switching.
- The focus is on becoming capable of designing, building, evaluating, deploying, and maintaining AI systems.

---

## Core Philosophy

Your learning loop should be:

> Read one good book → build one serious project → write what you learned → improve the project → move to the next layer.

Avoid scattered resources, certificate chasing, and passive reading. Every book should eventually influence a project decision.

---

# Long-Term AI Engineering Roadmap

The journey is divided into six phases.

| Phase | Duration | Main Focus | Main Project |
|---|---:|---|---|
| Phase 1 | Months 1–3 | ML Systems + Production ML | ML Prediction Service |
| Phase 2 | Months 4–6 | Deep Learning + Transformers | Transformer Text Classifier |
| Phase 3 | Months 7–10 | LLM Apps + RAG | Personal Knowledge RAG System |
| Phase 4 | Months 11–14 | Agents + Tool-Using AI Systems | AI Research Assistant |
| Phase 5 | Months 15–16 | LLMOps, Evaluation, Reliability | LLM Evaluation Dashboard |
| Phase 6 | Months 17–18 | Specialization / Flagship Project | Multimodal AI Research Copilot |

---

# Phase 1: Software + ML Engineering Foundations

## Goal

Become strong at building clean, maintainable ML-backed applications.

This phase should move you from notebook-based ML toward production-style ML engineering.

## Main Books

1. **Designing Machine Learning Systems** — Chip Huyen
2. **Machine Learning Engineering** — Andriy Burkov
3. **Designing Data-Intensive Applications** — Martin Kleppmann

## Key Concepts

Focus on:

- ML system design
- ML project lifecycle
- Data pipelines
- Feature engineering
- Batch inference vs real-time inference
- Training-serving consistency
- Model lifecycle
- Deployment
- Monitoring
- Reliability
- Databases and distributed systems basics

## Main Project: ML Prediction Service

Build a complete ML service, not just a notebook.

### Example Project

> Customer churn prediction API with training pipeline, model registry, FastAPI backend, Docker deployment, and monitoring dashboard.

### Required Features

- Data preprocessing
- Training script
- Evaluation report
- API endpoint
- Dockerfile
- Logging
- Basic monitoring
- README
- Architecture diagram

## Recommended Duration

2–3 months

## Final Output

By the end of this phase, you should have:

- A complete GitHub repository
- Clean README
- Data pipeline
- Baseline model
- Evaluation report
- FastAPI service
- Docker setup
- Tests
- Architecture diagram
- Technical write-up

---

# Phase 2: Deep Learning + Transformers

## Goal

Understand modern neural networks deeply enough to use, debug, and adapt them intelligently.

## Main Books

1. **Dive into Deep Learning** — Aston Zhang, Zachary Lipton, Mu Li, Alex Smola
2. **Deep Learning** — Ian Goodfellow, Yoshua Bengio, Aaron Courville
3. **Natural Language Processing with Transformers** — Lewis Tunstall, Leandro von Werra, Thomas Wolf

## Key Concepts

Focus on:

- Backpropagation
- Optimization
- Neural network training
- CNNs
- RNNs
- Attention
- Transformers
- Tokenization
- Embeddings
- Fine-tuning
- Evaluation

You do not need to read the Goodfellow book cover-to-cover. Use it as a reference when you want deeper math.

## Main Project: Transformer-Based Text Classifier

Build a clean NLP project.

### Example Project

> Research paper abstract classifier using transformer embeddings and fine-tuned models.

### Required Features

- Dataset collection
- Text preprocessing
- Baseline ML model
- Transformer model
- Fine-tuning
- Error analysis
- Model comparison
- Deployment as an API

## Recommended Duration

2–3 months

## Final Output

By the end of this phase, you should have:

- Baseline text classifier
- Fine-tuned transformer model
- Evaluation report
- Error analysis
- API endpoint
- README and documentation

---

# Phase 3: LLM Application Engineering

## Goal

Learn how to build real applications using foundation models.

This is the phase where you move from ML Engineer thinking toward AI Engineer thinking.

## Main Books

1. **AI Engineering** — Chip Huyen
2. **Hands-On Large Language Models** — Jay Alammar, Maarten Grootendorst
3. **LLM Engineer’s Handbook** — Paul Iusztin, Maxime Labonne

## Key Concepts

Focus on:

- Prompting
- Structured outputs
- Function calling
- Embeddings
- Retrieval
- RAG
- Evaluation
- Latency
- Cost
- Model selection
- Caching
- Safety
- Failure modes

## Main Project: Personal Knowledge RAG System

Build a serious RAG app.

### Example Project

> AI assistant for your resume, thesis, research papers, and notes.

### Required Features

- Upload PDFs
- Chunk documents
- Generate embeddings
- Store embeddings in a vector database
- Retrieve relevant chunks
- Generate answers with citations
- Show source passages
- Evaluate answer quality
- Track hallucinations
- Compare retrieval strategies

### Advanced Features

- BM25 search
- Vector search
- Hybrid search
- Reranking
- Query rewriting
- RAG evaluation
- Latency logging
- Cost logging

## Recommended Duration

3–4 months

## Final Output

By the end of this phase, you should have:

- Working personal RAG assistant
- Document ingestion pipeline
- Retrieval system
- Citation-based answers
- Evaluation dataset
- Retrieval comparison report
- Latency and cost tracking
- README and architecture diagram

---

# Phase 4: Agents and Tool-Using AI Systems

## Goal

Build AI systems that can take actions, use tools, follow workflows, and handle multi-step tasks.

## Main Books

1. **AI Agents and Applications** — Roberto Infante
2. **AI Agents in Action** — Micheal Lanham
3. **Designing Multi-Agent Systems** — Victor Dibia
4. **Prompt Engineering for LLMs** — John Berryman, Albert Ziegler

## Key Concepts

Focus on:

- Tool calling
- Function calling
- Agent memory
- Planning
- Reflection
- Task decomposition
- Multi-agent collaboration
- Human-in-the-loop systems
- Guardrails
- Agent evaluation

## Main Project: AI Research Assistant

This project fits well with your research and thesis background.

### Example Project

> An AI research assistant that reads papers, extracts methods/results/datasets/metrics, compares papers, and creates literature review tables.

### Required Features

- Upload research papers
- Extract title, authors, year, venue
- Extract methods
- Extract datasets
- Extract metrics
- Extract limitations
- Create comparison tables
- Generate literature summaries
- Ask questions across papers
- Export notes as Markdown/CSV
- Detect citation gaps
- Suggest related work sections

## Recommended Duration

3–4 months

## Final Output

By the end of this phase, you should have:

- Paper ingestion system
- Paper metadata extractor
- Method/dataset/metric extractor
- Literature comparison generator
- Research Q&A assistant
- Markdown/CSV export
- Evaluation notes
- README and demo

---

# Phase 5: LLMOps, Evaluation, and Reliability

## Goal

Learn how to measure, test, monitor, and improve AI systems.

This phase makes you more mature than someone who has only built chatbots.

## Main Books

1. **Reliable Machine Learning** — Cathy Chen, Niall Richard Murphy, Kranti Parisa, D. Sculley, Todd Underwood
2. **Designing Machine Learning Systems** — revisit selected chapters
3. **AI Engineering** — revisit evaluation, product, and deployment sections

## Key Concepts

Focus on:

- AI evaluation
- Regression testing
- Prompt versioning
- Dataset versioning
- Model monitoring
- Failure analysis
- Observability
- Human feedback
- Latency optimization
- Cost optimization
- Safety testing
- Production reliability

## Main Project: LLM Evaluation Dashboard

Build a dashboard to compare prompts, models, retrieval methods, and agent workflows.

### Required Features

Track:

- Accuracy
- Faithfulness
- Context relevance
- Hallucination rate
- Latency
- Cost
- Token usage
- User feedback
- Failure categories

## Recommended Duration

2–3 months

## Final Output

By the end of this phase, you should have:

- Evaluation dashboard
- Prompt comparison
- Model comparison
- RAG evaluation
- Failure taxonomy
- Latency and cost analysis
- Documentation and demo

---

# Phase 6: Specialization / Flagship Project

After the first five phases, choose a specialization.

Given your background, three strong options are available.

---

## Option A: AI Engineering for Research

Best if you want PhD/research alignment.

### Project

> AI Research Copilot for Computer Vision / Underwater Image Enhancement

### Features

- Read papers
- Extract methods
- Compare architectures
- Track datasets
- Suggest experiments
- Generate experiment reports
- Analyze metric CSVs
- Create plots
- Help write literature reviews

---

## Option B: Multimodal AI Engineering

Best if you want to combine computer vision and LLMs.

### Project

> Multimodal image analysis assistant

### Features

- Upload underwater images
- Analyze color cast, blur, contrast, and turbidity
- Compare enhancement outputs
- Generate natural-language evaluation
- Recommend enhancement method
- Explain image quality metrics

---

## Option C: Enterprise AI Systems

Best if you want industry AI Engineer roles.

### Project

> Enterprise Document Intelligence Platform

### Features

- Document upload
- OCR
- RAG
- Metadata extraction
- Summarization
- Approval workflow
- Access control
- Evaluation
- Admin dashboard
- Audit logs

---

## Recommended Flagship Project

The strongest long-term project for your profile is:

> **AI Research Copilot for Computer Vision and Underwater Image Enhancement**

It connects:

- Your computer vision background
- Your underwater image enhancement work
- RAG
- Agents
- Paper analysis
- Metric evaluation
- Experiment tracking
- Report generation
- Future PhD/research interests

---

# Suggested 18-Month Roadmap

| Months | Focus | Book Focus | Main Project |
|---|---|---|---|
| 1–3 | ML Systems | Designing ML Systems + ML Engineering | ML Prediction Service |
| 4–6 | Deep Learning + Transformers | Dive into Deep Learning + NLP with Transformers | Transformer Text Classifier |
| 7–10 | LLM Apps + RAG | AI Engineering + Hands-On LLMs | Personal Knowledge RAG |
| 11–14 | Agents | AI Agents books + Prompt Engineering | AI Research Assistant |
| 15–16 | Evaluation + Reliability | Reliable ML + AI Engineering revisit | LLM Evaluation Dashboard |
| 17–18 | Specialization | Selected references | Multimodal / Research / Enterprise AI project |

---

# Weekly Routine

Since you already have a job, keep the weekly routine sustainable.

## Weekdays

Spend 30–45 minutes per day.

Use weekdays for:

- Reading
- Taking notes
- Understanding concepts
- Small code experiments

Do not try to do heavy project work every day after work.

## Weekends

Spend 3–5 focused hours total.

Use weekends for:

- Project implementation
- Debugging
- Refactoring
- Writing documentation
- Creating demos
- Improving GitHub repositories

## Suggested Weekly Rhythm

| Day | Activity |
|---|---|
| Monday | Read + notes |
| Tuesday | Read + notes |
| Wednesday | Small code experiment |
| Thursday | Project implementation |
| Friday | Weekly recap |
| Saturday | Deep project work |
| Sunday | Refactor + document + plan next week |

---

# How to Read the Books

Do not read passively.

For every chapter, produce one of the following:

1. A short note
2. A diagram
3. A code experiment
4. A project improvement
5. A blog-style explanation

Examples:

- After reading about RAG evaluation, add a RAG evaluation module to your project.
- After reading about monitoring, add logging and dashboard metrics.
- After reading about embeddings, compare different embedding models.

---

# Book Priority List

Read in this order:

1. **Designing Machine Learning Systems**
2. **Machine Learning Engineering**
3. **Designing Data-Intensive Applications**
4. **Dive into Deep Learning**
5. **Natural Language Processing with Transformers**
6. **AI Engineering**
7. **Hands-On Large Language Models**
8. **LLM Engineer’s Handbook**
9. **Prompt Engineering for LLMs**
10. **AI Agents and Applications**
11. **Reliable Machine Learning**
12. **Designing Multi-Agent Systems**

Do not buy all at once. Pick one or two books per phase.

---

# Project Priority List

Build in this order:

1. **ML Prediction Service**
2. **Transformer Text Classifier**
3. **Personal Knowledge RAG System**
4. **AI Research Assistant**
5. **LLM Evaluation Dashboard**
6. **Multimodal AI Research Copilot**

Each project should have:

- Clean GitHub repository
- README
- Architecture diagram
- Setup instructions
- Demo screenshots or video
- Evaluation results
- Limitations section
- Future improvements section

---

# Final Strategy

The final strategy is:

> One book, one project, one written artifact per phase.

For every phase, produce:

1. Book notes
2. A working project
3. A technical write-up

Example for Phase 3:

- Notes from **AI Engineering**
- A RAG system over your thesis, papers, resume, and notes
- Blog/write-up: “Building a citation-based RAG assistant for research documents”

---

# Final Long-Term Direction

Your flagship project should eventually become:

> **AI Research Copilot for Computer Vision and Underwater Image Enhancement**

This can combine:

- RAG
- Agents
- Paper analysis
- Metric evaluation
- Image comparison
- Experiment tracking
- Report generation

This connects your job skills, MSc/research interests, thesis background, and future PhD ambitions into one coherent portfolio.
