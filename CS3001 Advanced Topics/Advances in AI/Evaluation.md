how can we evaluate QA systems?
- Benchmarking with metrics 
- LLM performance comparison e.g. latency
- Expert reviews of output depending on the context
- Repeat the same prompt multiple times to access clarity, readability, repeatability - and identify any bias or hallucinations
- AI judging acting as experts e.g. ChatBot Arena, LLMCompare

what metrics are there 
- [[ROUGE Metric]]
- BLEU Metric
- Accuracy 
- perplexity = how incoherent is the text 
- F1 score - balanced, considers both false positives and false negatives
- WER and CER for expected responses

why can't metrics alone be used (e.g. human evaluation)
- metrics cannot capture complexity and understanding of responses 
- determine the reasoning and synthesis quality 
- review responses that may be subjective
- identify out-of-vocabulary words 

areas where the model underperforms signals that more development is needed