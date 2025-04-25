![[Pasted image 20250421113936.png]]

[[Designing an LLM (Chatbot)]]
[[Applying a RAG Architecture]]

Decisions 
- choosing a vector database
- choosing an embedding model
- choosing an LLM

design consideration
- persona - a contract expert
    
- instruction - based on a telephone conversation, or question, supply information about a certain client or trade so that the traders can  
	- use previous contract to help lawyers structure and create new contracts
	- use previous contracts to help traders validate a client trade before execution
    
- context - it's too long for layers and traders to work together since it takes so long to read before executing the trade which causes them to miss out on profit 
	- need trade specific data like org type, countries covered
    
- format - parameter info e.g. fee amount: £XXXX - semi-strictly structured, not the same structure, but not excess text that is irrelevant information like: Certainly!
	- similar to JSON or table style
    
- audience - for lawyers to help them create the contracts, and for traders to help them understand the contracts
    
- tone - formal, for lawyers and traders to both use, need to focus on key information so the tasks can be done efficiently
    
- data - contracts from the cloud, the recorded telephone conversation 

### applying the rag architecture
1. choose a base LLM 
	-  closed source for proprietary information 
	- GPT-4 
		-  larger budget, pay for security - need to ensure usage agreements and privacy policy don't retain data and expensive, but probably worth it to make large profit trades
		 - better performance and larger context handling, needed for long lengthy contracts 
    
2. identify the RAG architecture
	- naive is the standard one
	- advanced does extra pre-processing steps to optimise the relevance and quality of the response
    
3. list the data sources used for the vector database
	- complex contracts that are stored in the cloud
    
4. create text chunks - makes it easier to process the information 
	- 500 - balance between response time and data quality
	- too small chunks leads to retrieval fragmentation where vital information is not included 
	- too large makes response more accurate but response time too long, can overload prompt and hurt retrieval precision

	https://hidevscommunity.medium.com/mastering-text-splitting-for-effective-rag-with-langchain-6f0757c5e02f
	- langchain to split the chunks 
	- Recursive splitter - splitting based on multiple separator patterns, progressively refining the chunking logic, handling documents with varied structures.
	- Scenarios requiring optimal chunking based on specific delimiters. e.g. contracts may have specific formatting styles and clauses

    
6. choose an embedding model and embedding block
	1. OpenAI Embeddings
	2. optimised for GPT models and works with Pinecone - API interface, 3 different models to choose from depending on price and embedding length
    
7. choose a vector database
	1. Pinecone
	2. FAISS - self hosted so more data security 
    
8. create a prompt embedding to find context
		1. context + instruction = prompt data
    
9. construct prompt input