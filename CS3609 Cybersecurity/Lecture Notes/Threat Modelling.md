what is threat modelling
- the process where threats are identified, explored and prioritised - taking a hypothetical attackers perspective and using models to find security problems

what does threat modelling allow us to do
- enables defenders to analyse attacker profile (goals), attack vectors (steps they follow), and the assets desired by the attacker
- identify high-value assets
- identify vulnerabilities
- identify most relevant threats - looking at the industry itself e.g. finance industry / healthcare
- identify any attack vectors that could go unnoticed - how an attacker can discretely enter a system e.g. supply chain attack → indirect attacks

who is involved in understanding the complexity of threats to be understood
- impossible for a single expert to exist so roles are broken up
	- red team - trying to break a system, but they still work for the organisation
	- blue team - defending the system against the red team and mitigate problems
	- specialised security experts for different domains e.g. physical infrastructure, human security, building architecture, network experts

when building a threat model, what need to be considered
- what are you building or analysing - network, system, application architecture
- what can go wrong - identify [[Threats]] → threat modelling e.g. ddos
- what can be done about it → [[Risk Analysis]] (using quantitative and qualitive risk analysis - risk register) , countermeasures, [[Controls]] 

how does threat modelling relate to the risk register
- threat modelling needs to occur first to actually identify the threats and assets - also needs to have prioritisation by most to least important asset-threat, so that the full risk register can be developed
  ![[Pasted image 20250422113453.png|500]]

what are the different threat modelling approaches 
- model the system being attacked
- model the attacker
- model the threats and attack vectors

how can the system being attacked be modelled (visualised)
- network diagram
- data flow diagram (context level diagram)
  ![[Pasted image 20250422114342.png|300]]
- software diagram (of the architecture to code)

how can the attacker be modelled 
- [[Persona-non-Grata (PnG)]]

how can the threats be modelled 
- with [[STRIDE Model]]
- with [[MITRE ATT&CK]] and mapping to the attack vectors
- [[Attack Trees]]

how do we choose an approach
- choose one  based on the system type, approach, and context 
- threat models can also be combined to more comprehensibly 
- ![[Pasted image 20250422122527.png]]

what are the basic steps of threat modelling 
1. produce a visual representation of the current situation of the organisation  (e.g. network diagram)
2. review intelligence that may highlight threats to the network diagram
3. identify possible techniques - left to right timeline on [[MITRE ATT&CK]] matrix
4. carry out [[Risk Analysis]] using [[CIA Triad]] to identify vulnerabilities and give hints to mitigations - create a Risk Register
5. select controls from [[MITRE ATT&CK]] or SANS, or if it happens, how to minimise the impact to ensure business continuity

can threat modelling process be automated
- difficult to do

what happens after threat modelling has identified all the threats 
- the gained cyber threat intelligence needs to be shared

why does cyber threat intelligence need to be shared
- cybercrime in one location in the world could spread to another organisation in a few days (including worldwide)

how can cyber threat intelligence be shared 
- must be described in a standardised way first so that different businesses can easily understand and analyse how it will impact them so that they can prepare and respond  

what standards are there to describe threats
- [[STIX]]
- [[MISP]]

how can a threat model be validated and assessed once it is described 
- by testing and simulation of controls and countermeasures e.g. simulating an attack
- [[Computational Simulation]]