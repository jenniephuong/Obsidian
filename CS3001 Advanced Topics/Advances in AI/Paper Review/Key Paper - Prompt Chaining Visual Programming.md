https://arxiv.org/pdf/2203.06566

LLMs using prompt engineering are customisable - can be easily customised at runtime to perform how the user expects without excess training, allowing non-ML experts to create LLM prototypes with minimal time and effort required, less expensive computation or data collection needed. 

Single prompts often to simple to reflect the user's needs for complex applications or use cases, so prompt chaining is used instead.
- prompt chaining was shown effective in completing complex tasks, but user's still need support when creating their own LLM chains

PromptChainer is the proposed solution - a visual interface to build LLM chains in combat to the 3 main struggles people have due to how extensive LLMs are 
1. the overhead of fully utilizing LLM capabilities
2. the tendency of inadvertently introducing errors to the chain when prompting - accidentally causing the LLM to produce the output in an unexpected format and thus causing errors that break the entire chain, or cascade down to further sections of the chain. 
3. the cascading errors caused by blackbox and unstable LLM generations.

Interfaces has
- nodes - aka. LLMs that users can implement with certain inputs and outputs 
- helper nodes - aka. any functions that support data formatting / transformation or evaluation 
- communication nodes - exchanging data with the real world, calling external APIs

Allows users to test and evaluate each node individually, and run the whole chain at once to assess the output from each node 
- very modular and considers each node independent of another 

Conducted user testing with users trying to build their own chains 
- LaMDA base LLM used

Results 
- able to create parallel logical branches chains and also incremental iteration chains 
- can be used to make chains that single prompts can't handle, but also generalise single prompt outputs so they can be used in wider contexts 
- works with both a top down and bottom up approach to building the LLM chains 
- visually building the chains can help user's identify fundamental flaws with their initial prompt chain idea 
- trying to track multiple independent but parallel chains can be complex to do
- trying to combine interdependent parallel tasks reduces coherence overall, as each node works individually with no awareness on what the other nodes are doing (e.g. story generate chain creating each paragraph in parallel )

Limitations 
- because prompts were pre-decided, people could be too invested in their first LLM chain architecture, could be better to allow them to rapid prototype chain architectures without getting too invested 
- needs to be investigated more with tasks that aren't as easy to functionally decompose (aka. split up the functionality into steps)


the UI looks like this  - an example of a user built prompt chain by piecing together nodes 
![[Pasted image 20250310120601.png]]

My thoughts
- I didn't realise the errors that can exist when doing prompt chaining, whilst a working chain is very effective, poorly created chains are almost worst than single prompts, as they can cause the LLMs to go completely off track. 
- Could these tools also be used for demonstrations, for example if creating a QA software for a company, using these visual tools can help designers and develop build rapid prototypes to show to the client to ensure they match spec. 
	- actually - what is the main purpose of this, for prototyping or true developing?? 
	- if for prototyping, wouldn't effort be wasted a bit since models are not deterministic. 

- **"Provides scaffolds for building a mental model of LLM's capabilities"**: It helps users understand how the LLM works by offering support structures (like templates or guides) to visualize and conceptualize the model's capabilities.
- **"Handling arbitrary LLM data formats"**: The tool is designed to work with various data formats that LLMs might produce or require, ensuring flexibility.
- **"Defining a 'function signature' for each LLM step"**: This means specifying the input and output structure for each step in the LLM process, much like defining functions in programming.
- **"Debugging cascading errors"**: When a sequence of operations has errors that propagate or compound across the chain, PromptChainer helps users identify and fix them effectively