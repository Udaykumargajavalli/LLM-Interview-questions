# LLM-Interview-questions

A collection of interview questions covering large language models, retrieval-augmented generation (RAG), and related systems.

## Topics

- [RAG](RAG/readme.md) — retrieval and generation troubleshooting, embedding evaluation, multi-document retrieval, and scaling vector stores.
- [Model architecture](model-architecture.md) — Transformer components, attention, normalization, model families, and related concepts.
- [Agent systems](agent.md) — agent architectures, memory, state management, tools, and multi-agent collaboration.
- [Document processing](document-processing.md) — chunking strategies.
- [Evaluation and monitoring](evaluation-monitoring.md) — ranking metrics, evaluation approaches, and diagnosing system failures.
- [Fine-tuning](fine-tuning.md) — LoRA, parameter-efficient methods, and fine-tuning strategy.
- [Inference optimization](inference-optimization.md) — KV cache, GPU memory, quantization, and inference frameworks.
- [Knowledge graphs](knowledge-graph.md) — GraphRAG principles and knowledge-graph challenges.
- [Prompting](prompting.md) — zero-shot failures, prompt versioning, and consistency testing.
- [Embeddings and vector search](embeddings-vector-search.md) — similarity search, vector database choices, and hybrid retrieval.
- [Production engineering](production-engineering.md) — budget-aware design, real-time summarization, notebook productionization, and safe deployment.
- [Machine learning implementation](machine-learning.md) — building a pipeline with NumPy and Pandas.

## RAG interview questions

The [RAG question set](RAG/readme.md) covers:

1. Investigating incorrect answers and proving the root cause.
2. Diagnosing poor answer quality when retrieved documents are relevant.
3. Measuring whether embedding improvements help the system.
4. Retrieving and assembling context from multiple documents.
5. Identifying bottlenecks and redesigning a vector-store architecture as it scales.
6. Improving latency, evidence quality, contextual precision, chunking, and retrieval freshness.
7. Selecting a vector database for RAG over ten million documents.