https://www.scribd.com/document/827113694/Comparative-Analysis-of-RAG-Fine-Tuning-and-Prompt-Engineering-in-Chatbot-Development#:~:text=expand%20document%20information-,This%20paper%20compares%20the%20effectiveness%20of%20Retriever%2DAugmented%20Generation%20

Specifically for chatbot / QA systems with question answer pair dialogue 

[[Advances in AI/Evaluation]] metrics used 
- Accuracy - % of correct responses
- BLEU - compares overlapping n-grams between generated and reference, common for translation 
- Perplexity - how well the LLM can produce a sequence of words, low = more coherent text
- Human evaluation - quality, relevance, coherence, application to various scenarios 

|     | Tech Stack                                                                                                       |
| --- | ---------------------------------------------------------------------------------------------------------------- |
| RAG | - langchain<br>- used a Mistral model to create the numerical embeddings<br>- stored in a Milvus vector database |
| FT  | - Llama LLM <br>- transformers                                                                                   |
| PE  | - langchain with conversation buffer history                                                                     |

![[Pasted image 20250310151612.png]]

##### Results 
- Fine-tuned performed the best across all metrics - most effective for generating relevant and coherent responses specific to the dataset, minimal uncertainty and high understanding of the task
- RAG second, but the higher perplexity shows that it's not as robust when responding to unexpected queries
- Prompt engineering the worst - despite being cost-effective and flexible, performed worse on accuracy and BLEU - less effective, but not totally useless, still provided a good user experience 

Need to balance the effectiveness with the resources available 
- large high quality specialised datasets and computational power, fine-tuning will provide the most accurate results 
- limited resources - prompt engineering more viable
- middle ground - RAG, especially for real time data retrieval needs, or continuously updating knowledge 

how can we decide? 
- based on data - slow moving or continuous update 
- industry - fine-tuning is good for specialised or nuanced terminology like legal document summariser with legal jargon
- sources - RAG gives more transparency by providing sources which could be more important for ethical concern products e.g. insurance, retail customer service, finance
- past data - if past data is available then fine-tuned is more suitable to understand new prompts better

##### Future works 
- combing fine-tuned and RAG is probably the best approach, but still expensive to implement this hybrid approach 
- adaptive prompts that understand the nuance of a response  
- bias and ethical considerations need to be made 
- applying these technologies to the real world need to ensure that the accuracy is not sacrificed to keep the chatbot sophisticated

##### Risks
- computationally expensive
- lack of appropriate training data