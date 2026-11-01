# Production Engineering Interview Questions

1. You have a $10,000 monthly budget for AI infrastructure. Design a recommendation system that scales.

   Discussion points: Estimate workload and unit costs, consider build-vs.-buy decisions, compare simple baselines with more complex models, and plan incremental deployment within the budget.

2. How would you build a system that summarizes customer support tickets in real time?

   Discussion points: How would you handle different ticket formats, control summary quality, measure whether summaries are helpful, handle an LLM service outage, and collect feedback for improvement?

3. Here is a Jupyter notebook that works. How would you productionize it?

   Discussion points: Cover error handling and logging, configuration management, testing, deployment, monitoring, and documentation.

4. Walk through deploying a GenAI service with FastAPI, Docker, and Kubernetes. How would you ensure rollback safety?
5. If your system exceeds its budget because of model size, how would you decide among speed, accuracy, and cost trade-offs?
