> the practice of designing inputs for generative AI tools that will result in better outputs without altering the model's parameters or expanding its knowledge base

requires an understanding of 
- the domain to incorporate the goal into the prompt like what good or bad responses look like. 
- AI models as different models will respond differently to the same prompt 
	- best to create a prompt template that can be programmatically modified according to some dataset or context ![[Pasted image 20250310161826.png]]
many prompt engineering tools are becoming available. 

![[Pasted image 20250224171855.png]]
using techniques like context, decomposition, learning, shot-based

goal: lead the model to deliver the results that use user wants


what are the types of prompt engineering
- [[Shot-based Prompting]]
- [[Prompt Chaining]]
- Chain of Thought Prompting
- [[Prompt Structuring]]


##### Pros
- cost-effective -> least time consuming or resource intensive and basic prompt engineering can be done manually 
- flexible to modify 
- quick to develop - e.g. for rapid deployment scenarios 
- most flexible and effective for open-ended situations where there are a diverse array of potential outputs like image and video generation

##### Cons
- less effective in proving coherent and accurate results compared to more advanced techniques like RAG or fine-tuning [[Sub Paper - Comparing RAG, Fine-Tuning, and Prompt Engineering for Chatbot development]]

#flash 

