> models that have been trained of a large volume of data (text) in order to predict the next tokens 

this developed into Large language models using [[Transformers]] based deep learning architecture - great for natural language processing 


LLMs prompts are not restricted to only text, but can include other multi-media like image or audio, but for [[QA Systems]], prompts are primarily text, requires an instruction or a question (optionally, input data and examples). Prompts and responses can be improved using [[Prompt Engineering]]

- long range dependencies and contexts
- 2 types :closed vs, open llms
    - business model requiring license and payment monetisation
    - open to programming community for fine tuning

using LLMs for different industries require different techniques, or using LLMS tuned on industry specific data

what optimisation methods exist for organisations to optimise model behaviour
- https://www.ibm.com/think/topics/question-answering
- [[Fine Tuning]]
- [[Prompt Engineering]]
- [[Retrieval-Augmented Generation (RAG)]]

##### Cons 
despite being popular, LLMs have many limitations 
- poor adaptability to having out-dated training data 
- too generalist, hard to adapt them to specific use cases and enterprise applications 

- ==stochastic== response - randomly determined to some extent even when re-using the same prompt - deal with this by tweaking the temperature parameter, but this alone is not enough to prevent unwanted variability in responses

#flash 