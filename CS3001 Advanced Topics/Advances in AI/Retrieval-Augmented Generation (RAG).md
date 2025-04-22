> an advanced, specific data architecture framework / technique for retrieving facts from an external knowledge base to optimise LLM responses on the most accurate and up-to-date information. 

consists of three parts 
- knowledge base 
- retriever
- LLM

gets context in order to made a decision based on the context, not generic to anybody who asks the prompt

![[Pasted image 20250224175612.png]]

1. ==query==: user submit a query to the LLM (initially the prompt goes straight to LLM)
2. ==information retrieval==: instead, an algorithm or API is used to retrieve relevant information first from the [[Vector Databases]]
3. ==integration==:  combine the retrieved data with the user's query to produce and augmented query, and then give it to the LLM
4. ==response==: LLM generates an accurate response based on retrieve data and own training knowledge, this allows the LLM to give evidence for why it gave a certain response 

Different types of RAG
- naive
- modular
- advanced

Aim - improves retrieval and generation and guide the LLM to produce relevant and accurate outputs 
Knowledge - integrated knowledge as needed 
Up-to-date - integrated latest knowledge 
Transparency - transpired as it uses sourced data 
Domain specificity - can adapt to domain as new sources are added 
Resource use - user driven resource cost, datasets and pipelines to connect the LLM to the dataset need to be constructed 

Solves common issues with regular [[Large Language Models|LLM]] use
- regular LLMs have no source to derive their responses from, so information can be inaccurate - LLMs are directed to focus on primary source data, so less likely to leak data or hallucinate
- information given can be out of date, instead of having to retrain the entire model for new information, augment the data store with updated information. much less computational effort required. 
	- any info can be part of the corpus, documents, PDFs, anything relevant to the business operations
- hallucination from not knowing the answer and giving something random - encourages the LLM to admit when it doesn't know things based on what is or is not available in the vector database (but this can be a negative effect if the initial user prompt doesn't get an answer despite being answerable)

Can be built using langchain 

##### Pros 
- best for dynamic data sources like databases 
- best for trust essential systems (because of sources and less hallucinations) and for systems where accurate, relevant, and current information is essential
	- for ethical concerns 
- good use cases include documentation chatbots
- allows non-public data to be leveraged 

##### Cons
- How we determine and select which information needs to be considers, as a poor calculation of similarity between the prompt and sources will produce inaccurate responses  
- not enhancing the base model itself
- requires extensive data architecture construction and maintenance to build the pipelines between the organisation's data and the LLM 
- need to have precise prompt engineering to locate the right data and ensure the LLM can handle it properly 
- not as robust to unexpected queries 