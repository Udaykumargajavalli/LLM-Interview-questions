# RAG Interview Questions

## 1. Diagnosing Incorrect Answers

A RAG system that has been performing well suddenly starts returning inaccurate answers. How would you investigate the problem from the user query through retrieval, context construction, and generation? What evidence would you collect to identify the root cause and distinguish it from a symptom?

## 2. Relevant Retrieval, Poor Answers

The retriever returns documents that appear relevant, but the generated answers are still poor. What could be going wrong between retrieval and generation, and how would you isolate the cause? Consider how document chunking, ranking, context assembly, prompt instructions, and conflicting evidence might affect the result.

## 3. Evaluating Embedding Improvements

You are considering a new embedding model for a RAG system. How would you determine whether it actually improves the system? Describe the evaluation data and metrics you would use before and after the change, including how you would assess retrieval quality separately from final answer quality.

## 4. Retrieving Evidence Across Multiple Documents

A user asks a question whose answer depends on information spread across five documents. How would you design retrieval and context construction to find and combine the necessary evidence? How would you handle missing or conflicting information, and evaluate whether the final answer is complete and well-grounded?

## 5. Scaling a Vector Store

A RAG system works well with 10,000 documents, but the corpus grows to one million. What bottlenecks would you investigate first, and how would you redesign the indexing and retrieval architecture? Explain the trade-offs your design makes among relevance, latency, cost, and data freshness.

## 6. Slow but Accurate Retrieval-Augmented Generation

You inherit a RAG system that users say is slow but accurate. How would you diagnose and improve it?

Discussion points: Measure latency across query processing, retrieval, reranking, context construction, and generation before optimizing. How would you preserve answer quality while evaluating latency and cost trade-offs?

## 7. Verifying Retrieved Evidence

After retrieval, how do you know whether the retrieved documents or paragraphs are correct? Distinguish relevance from factual correctness, source authority, freshness, and consistency with other evidence.

## 8. Missing Company-Specific FAQs

Your RAG chatbot answers general questions well but fails on company-specific FAQs. What might be wrong with your retrieval setup? How would you check ingestion coverage, access filters, terminology, embeddings, and retrieval ranking?

## 9. Too Many Irrelevant Chunks

If a retriever returns too many irrelevant chunks, how does that affect the final LLM answer? How would you improve filtering, ranking, and context selection without losing necessary evidence?

## 10. Chunk Size Trade-offs

What trade-offs do you face between smaller and larger context chunks in RAG? Consider retrieval precision, semantic completeness, overlap, context-window usage, and cost.

## 11. Keeping Retrieval Fresh

Your RAG system answers correctly in development but fails in production when documents are updated frequently. How would you maintain retrieval freshness? Consider incremental indexing, updates and deletions, versioning, cache invalidation, and freshness monitoring.

## 12. High-Similarity but Contextually Irrelevant Results

Your retriever returns high-similarity junk. How would you improve contextual precision?

Example: A query asks, "How do I enable two-factor authentication in Gmail?" but retrieval returns documents about multi-factor authentication in Microsoft Teams. The passages have overlapping concepts but the wrong product context.

Discussion points: Compare semantic chunking, query rewriting or expansion, HyDE, query routing, rerankers, and domain-adapted embeddings. How would you preserve product-specific constraints and verify that changes improve contextual relevance rather than embedding similarity alone?

## 13. RAG over Ten Million Documents

Your team needs to build RAG over 10 million documents. Which vector database would you recommend, and crucially, why? Explain the trade-offs, including the number of chunks and vectors, metadata filtering, recall, latency, index memory, update rate, sharding, operational complexity, and cost.

For related questions, see [embeddings and vector search](../embeddings-vector-search.md) and [fine-tuning](../fine-tuning.md).
