#lecture

In order to secure systems, we need to consider 
- how will security be evaluated 
- securing the architecture
- secure coding 

but why do we need to secure systems
- there are many cyber security breaches that compromise affect systems
- every day a system faces [[Threats]] so we need to protect [[Assets]]

- 1986 - Pakistani Brain - the first malware 
- Killer USB, key logging USB
- sophisticated security threats - IoT / Malware / Ransomware-as-a-Service - freely available ransomware for distribution without needing to program it yourself 
- deepfakes 

how do enterprise companies secure and evaluate their security 
- using the [[Security Review Cycle]]

there are many complexities in enterprise systems because each system differs in architecture, how we design the software poses risks

what are the different types of system architectures
- [[Specific Component Types]] - not really a type, but talks about the risks involved
- [[Mobile and IoT]]
- [[Monolithic Architecture]]
- [[Microservice Architecture]]

how actions can be done to secure systems - software engineering approaches that include cyber security elements
- processes - change management + quantitative analysis
- ***monitoring*** the architecture with software ([[Intrusion Detection Systems (IDS)]])
- Securing the code itself ([[Mobile and IoT]])
- [[Code Analysis]]  
- [[Software Testing]] 
- [[System Testing]]

how do we know which areas of the system to focus on securing 
- by conducting a Quantitative Analysis 
- e.g. for each device, network, software, data, plot it against a probability impact graph to see which areas need to be focused on most (where probability = risk)
- ![[Pasted image 20250415174811.png|500]]

how can security be implemented for a designed / developing systems
- risk review at every stage
- design review - ensure the design of the system matches the requirements and technology
- code review 
- code management (control) - includes version control on github 
- code analysis
- code testing
- system testing (attacks)

how can security be implemented for working (existing and live) system
- pattern or signature-based intrusion detection system (IDS) - involve people already using the system. when traffic coming into an organisation, patterns can be detected to detect suspicious behaviour
- anomaly-based intrusion detection system (IDS)
- traffic-based methods
- protocol patterns
- testing (DR or other recovery)
- machine access (control)