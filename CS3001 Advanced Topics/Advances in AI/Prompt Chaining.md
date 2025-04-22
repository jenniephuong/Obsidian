> technique of proving a series of prompts to an NLP model to guide it to produce the desired response - where the output of one LLM becomes the input to another

##### single vs complex prompts 
single prompts contain a single question or instruction while complex prompts contain multiple instructions or questions where the model needs to perform a series of actions to provide a detailed response. 

prompt chaining is used to simplify complex prompts
- instead of giving one complex prompt, split up the complex prompt into multiple single prompts and chain them together
- e.g. extract and categorise - get output
    - extract first - get output
    - categorise - get output

![[Pasted image 20250224173224.png]]

##### pros of prompt chaining 
- traceability - allows users to understand the steps required to complete a request than a large monolithic prompt
- accuracy and clarity - reduce the risk of errors or misunderstandings, can understand better and larger contexts and outperform monolithic prompts 
- troubleshooting - easier to identify at what point in the chain needs adjustments to produce optimal responses, more granular control
- consistency - forcing the model to follow a series of prompts maintains consistency in tone or style or format which might be needed
- widely applicable - most tasks can be functionally decomposed (although not all), making chaining a good solution
	- multiple instructions
	- multiple output transformations
	- when models seem to lose focus or forget context

##### cons of prompt chaining 
- management difficulty - interrelated prompts can be hard to manage when the china becomes long or intricate, more room for error especially when using different AI models 
- hyper-dependency on the first prompt, if the initial prompt is bas then the failures will cascade throughout the rest of the chain 
- time consuming, the quality of each chain link needs to be (iteratively) tested and reviewed
- longer processing time - multiple LLM calls instead of 1
- higher costs - each part of the chain requires an LLM call which leads to higher costs for tokens for API usage (especially since prompt chaining produces longer outputs than one big prompt)


##### applications 
- structured prompt chains used for customer service chatbots, where prompts are linked together so the system can build upon previous responses and maintain context 
- any sort of multi step tasks like programming development, personalised recommendations, content creation from outline to editing

but how can non-AI experts build prompt chains - perhaps through a visual interface?
[[Key Paper - Prompt Chaining Visual Programming]]