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
