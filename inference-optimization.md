1. How is the space complexity of KV Cache calculated?
2. What are DeepSpeed's core features and architecture, and how do you use it?
3. How does Flash Attention's underlying principle work?
4. What are the principles behind GPU memory optimization techniques, and how do they compare?
5. How do you comprehensively choose an LLM inference framework?
6. How large is a 13B model after INT8/INT4 quantization?
7. How do you handle very long context windows?
8. How would you redesign a decoder-only Transformer's attention mechanism to make inference faster and more memory-efficient without hurting quality too much?

   Discussion points: Consider Grouped Query Attention (GQA). Keep separate query heads while sharing key and value heads within groups; for example, use 16 query heads with four key/value heads. Compared with standard multi-head attention, this reduces KV-cache memory and decoding memory bandwidth, but does not reduce query-head attention computation proportionally. How would you measure the quality and latency trade-offs?

9. You can have fast, cheap, or accurate models. Pick two and explain why. Under what workload could you improve all three rather than treating this as a strict constraint?
10. Compare top-K sampling, top-P sampling, and temperature. How do they interact, and when would you choose each?
11. What is "context window waste," and how would you reduce it?
