![[Pasted image 20250224171131.png]]

Step 1: Choose a base LLM - open or closed source model?
- in the exam we can choose any model as the base LLM since we won’t have access to huggingface
- e.g. GPT - large model and very popular in many industries

Step 2: Identify the RAG architecture (naïve, modular, advances, etc.) 

Step 3: List data sources that will be used for the vector database 

Step 4: Create text chunks - define text size and text chunk block 
- word by word, paragraph by paragraph, document by document
- what are the implications of each option

Step 5: Choose an embedding model and the embedding block

Step 6: Choose a vector database

Step 7: Create a prompt embedding to find context -basically a way to combine the input such that **==prompt input data = instruction (og prompt) + context (vector db)==**

Step 7: Construct prompt input