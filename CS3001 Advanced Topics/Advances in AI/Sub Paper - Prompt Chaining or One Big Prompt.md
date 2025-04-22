https://www.prompthub.us/blog/prompt-chaining-guide
https://arxiv.org/pdf/2406.00507

[[Prompt Chaining]]

>TLDR; prompt chaining outperforms one big prompt, it's better to have concise, single function prompts so that there is no negative influence on the model

compares a prompt chain approach with a stepwise approach across 3 task types 
- creating a draft
- critiquing a draft
- refining a draft 

![[Pasted image 20250421181319.png]]

uses LLMCompare as an evaluation
- quality of summary
- pinpoint missing information
- pinpoint irrelevant information
also used human evaluators on the same principles

results 
- the refinement always improved upon the initial draft in both cases 
- prompt chaining is better for producing summaries
- initial summaries were worst with stepwise, however this could be because the stepwise approach influenced how the first draft is created since the model can anticipate the refinement needs to be done
- prompt chaining summaries were longer than stepwise ones
