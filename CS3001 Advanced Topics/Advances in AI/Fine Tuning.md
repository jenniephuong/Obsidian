> adapting a model for a specific task or use case, using the broader knowledge gained from pre-training and honing it towards specific concepts

models can be fully fine tuned 
- update all parameters 

or parameter-efficient fine tuned
- updates only the most relevant parameters
- allows for the fine-tuning to occur on lower spec hardware


![[Pasted image 20250224165902.png]]

Pipeline steps 

1. pre-training
2. fine-tuning
3. quantizing 

goal is to improve performance in specific use cases 
Aim - adapts pre-trained LLM models with new content to suit a particular task or application domain
Knowledge - limited to knowledge in base model
Up-to-date - static - expensive to extend
Use cases - more general tasks and applications 
Transparency - less transparent
Domain Specificity - fine-tuned to specific domains 
Resource use - upfront cost for fine-tuning 

Pre-training uses large datasets while fine tuning uses smaller datasets

![[Pasted image 20250224171923.png]]


![[Pasted image 20250224171941.png]]

##### Pros
- gives us greater influence in how the model behaves and reacts since the context is baked into the weights instead of being supplemented on top as an extra technique
- better for speed when running the model - smaller prompt context windows to still get the best responses for specific use cases 
- good for when datasets are available, specific industries that have easily identifiable patterns (specific jargon) 
- can produce highest accuracy in [[Sub Paper - Comparing RAG, Fine-Tuning, and Prompt Engineering for Chatbot development|Chaubey et al.'s]] comparison paper and outperform their base models 

##### Cons 
- information cut-off (outdated)
- upfront resource cost data preparation and training processes are so compute-intensive and time-consuming -> powerful GPUs running in parallel and large memory to store the fine-tuned LLM
- poor generalisation, can't be used in multiple application, only for the specific application it was fine tuned for
- poor datasets will impact the effectiveness of the final model

#flash 