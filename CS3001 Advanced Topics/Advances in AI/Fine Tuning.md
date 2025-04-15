> adapting a model for a specific task or use case, using the broader knowledge gained from pre-training and honing it towards specific concepts

![[Pasted image 20250224165902.png]]

Pipeline steps 

1. pre-training
2. fine-tuning
3. quantizing 

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

##### Cons 
- information cut-off (outdated)