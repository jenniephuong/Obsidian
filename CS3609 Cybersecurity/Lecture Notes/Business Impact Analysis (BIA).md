what is a business impact analysis
- identifies the resources and controls that should be implemented as a result of an interruption caused by a cyber incident.


what questions need to be asked as a cs expert when conducting BIA
- What is the impact on the business? 
	- e.g. impact of a stolen computer
- Which business functions are affected by the incident?
	- e.g. isolated or knock-on effect
- How Critical are these Business Functions and their associated information systems? (CBF)
- What are the Critical Dependencies? (CD)
- What is the Maximum Tolerable Downtime? (MTD) 
	- e.g. if amazon is down for 1 min, how much money are they losing, so they’ll create a MTD of 5 seconds which is tolerable loss
- What is the Recovery Time Objective? (RTO) 
	- every critical function can go down, how long does it take to bring it back up
    - RTO < MTD
- What is the Recovery Point Objective (RPO)?
	- how much can the organization afford to loose when the system goes down before recovery is needed

what is the best way to approach BIA 
- use [[Value Chain]] analysis to determine CBF and CD (what are the assets)
- conduct [[SWOT Analysis]]
- after this, do risk management: conduct [[Risk Analysis]] and produce a [[Prioritised Risk Register]] for all assets in the CBF and CDs.