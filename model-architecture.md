# Model Architecture Interview Questions

1. How is BERT+CRF jointly trained?
2. Why are decoder-only models dominant today? When would an encoder-decoder model be a smarter choice?
3. What's the core difference between GPT and BERT?
4. How are MLA and KV Cache used?
5. How does multi-head attention work, and what are the pitfalls of splitting QKV?
6. Why is positional encoding important?
7. Why did LLaMA choose RMSNorm?
8. Why does DDPM randomly sample timesteps?
9. RMSNorm vs. LayerNorm: how do they compare in training efficiency?
10. How do you choose between CNN, RNN, and Transformer?
11. How does logistic regression work?
12. How does parameter scale affect large models?
13. How do encoders and decoders work, and what is the functional difference between them?
14. How does MoE improve agent capability?
15. What are VQ-VAE's principles and full architecture?
16. RMSNorm vs. LayerNorm: how do they compare in numerical stability?
17. How do you manage VQ-VAE codebook collapse?
18. Does autoregressive generation use token IDs or probability distributions?
19. Explain attention in plain English. Where do queries, keys, and values come from, and how are they computed and used in self-attention and cross-attention?
20. What are the core components and principles of the Transformer architecture?
21. What does tokenization really mean, beyond just "splitting text"?
22. Can you implement byte pair encoding (BPE) to tokenize text data? Show how you learn merge rules, apply them to new text, and handle unseen input.
23. Why can chain-of-thought (CoT) reasoning improve LLM performance on complex tasks, yet sometimes fail catastrophically? How would you evaluate correctness rather than trusting a plausible explanation?
