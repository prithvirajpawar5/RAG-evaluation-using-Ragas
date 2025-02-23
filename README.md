How Do We Evaluate RAG Using Ragas?

Evaluating RAG (Retrieval-Augmented Generation) means assessing how effectively a system retrieves relevant information and how accurately the LLM (Large Language Model) generates responses based on that information.

Ragas is a framework that provides objective evaluation metrics to measure the performance of LLM/RAG applications. These metrics help assess both the retrieval and generation components of your AI system.

Key Metrics for Evaluating RAG

1. Context Precision – Measures how many retrieved chunks are relevant.
e.g. A legal AI retrieves 10 case laws, 6 of which are relevant → Precision = 60%.

2. Context Recall – Evaluates how many relevant documents were retrieved.
e.g. A medical chatbot retrieves 8 out of 10 relevant papers → Recall = 80%.

3. Response Relevancy – Assesses if the response directly answers the query.
e.g. “What are the symptoms of flu?”
- “Flu symptoms include fever, cough, sore throat.” (High Relevancy)
- “Flu spreads through droplets.” (Low Relevancy)

4. Faithfulness – Ensures the response is factually consistent with the retrieved context.
e.g. Retrieved Context: “The Eiffel Tower was completed in 1889.”
- “The Eiffel Tower was completed in 1889.” (Faithful)
- “The Eiffel Tower was built in 1850.” (Not Faithful)

To thoroughly evaluate an AI system, we need high-quality reference datasets. For example in a Q&A-based RAG, a strong dataset consists of well-curated question-answer pairs that:
- Contain diverse real-world queries
- Cover a broad range of scenarios
- Have enough samples to ensure statistically meaningful evaluation
- Are regularly updated to avoid data drift

Manually curating high-quality datasets is time-consuming and expensive. Ragas offers tools to generate synthetic test datasets using LLMs and embedding models, making evaluation more efficient.

 I’ve created a hands-on tutorial on RAG evaluation and test data generation using Ragas. Access it for free on GitHub!