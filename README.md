# Ahmed Elsayed

AI / Machine Learning engineer in Cairo, working on LLM fine-tuning, evaluation and RAG.
Open to junior AI / LLM engineering roles, on-site in Cairo or remote.

[LinkedIn](https://linkedin.com/in/ahmed-elsayed16112002) · [Email](mailto:elmo7andes@gmail.com)

## Projects

### [WhatsApp Twin](https://github.com/ahmed-elsayed1611/Twin_project/tree/main/whatsapp-twin)

A 3B-parameter Egyptian-Arabic chat model fine-tuned on my own private conversation data.

| Stage | Result |
|---|---|
| Data preparation | 135,289 raw lines → 26,989 multi-turn samples, with PII redaction and a leakage-free split |
| Supervised fine-tuning | LoRA on NileChat-3B: validation loss 1.625, against 1.734 for Qwen2.5-3B |
| Preference alignment | DPO with hard negatives from my own replies: held-out accuracy 68.7% → 71.3% |
| Evaluation | LLM judge in both A/B orders prefers the DPO model in 71% of decided pairs (p = 0.0003) |

No data, weights or generated text are in the repository. The code, tests and write-up are.

### [LLM Twin — reference system](https://github.com/ahmed-elsayed1611/Twin_project)

The production-style architecture from *LLM Engineer's Handbook*, studied and run: data
collection into MongoDB, a ZenML feature pipeline into Qdrant, and RAG retrieval with query
expansion, self-query filtering and reranking. Deployment and MLOps stages are in progress.

### [Mini-RAG](https://github.com/ahmed-elsayed1611/MIni_Rag)

A FastAPI document question-answering service with swappable LLM and vector-database
providers, on PostgreSQL and PGVector. Built following a course.

## Publication

**Evaluating Student Performance Prediction Using Machine Learning Models**<br>
Port-Said Engineering Research Journal, 2025 · co-author ·
[doi.org/10.21608/PSERJ.2025.387085.1412](https://doi.org/10.21608/PSERJ.2025.387085.1412)

Regression (XGBoost, Random Forest, SVR) reached R² 0.930; classification reached 89.4% accuracy.

## Stack

**LLMs:** PyTorch, Hugging Face Transformers, PEFT, TRL, Unsloth, Sentence Transformers, LangChain<br>
**Pipelines and serving:** ZenML, FastAPI, Docker, GitHub Actions<br>
**Data:** Qdrant, MongoDB, PostgreSQL / PGVector, SQLAlchemy, Pandas, scikit-learn, XGBoost
