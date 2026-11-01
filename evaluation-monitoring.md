

1. How is NDCG calculated?
2. How do you choose between automatic and human evaluation?
3. How do you mitigate LLM hallucination and safety risks?
4. Which modules in an agent system are most prone to failure?
5. How do you locate the root cause of RAG errors?
6. How do you diagnose knowledge-based vs. behavior-based errors?
7. How do you choose among training, inference-time, and knowledge-augmentation approaches (for hallucination mitigation)?
8. How is MRR defined in RAG?
9. Can we trust one LLM to evaluate another LLM's output?

   Discussion points: Use LLM judges cautiously, not blindly. They can provide fast, inexpensive, scalable judgments, but may reward fluency over factuality and share biases or blind spots with the model being evaluated. An eloquent hallucination may score above a plain but correct answer. How would you calibrate judges against human review and reference-based checks, especially for truthfulness, safety, and creativity?

10. Your model works well Monday through Friday but performs poorly on weekends. How would you investigate?

    Discussion points: Examine data distributions, traffic patterns, monitoring, and upstream dependencies before attributing the issue to the model.

11. A production model suddenly drops from 95% to 60% accuracy. Walk through your investigation.

    Discussion points: Check the data pipeline and upstream changes first, verify that monitoring and labels are reliable, compare distributions rather than accuracy alone, and have a rollback ready before investigating.

12. How would you detect and monitor hallucinations in production?
13. Which metrics matter most in an evaluation pipeline?
