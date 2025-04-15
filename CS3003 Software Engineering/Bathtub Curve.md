> The visual representation of the [[Evolution]] and lifetime of a system, and how a product's failure rate changes over time - applicable to every system

what are the phases of a bathtub curve

![[Pasted image 20241104101900.png]]

- **infant mortality failures** → many failures when the system initially goes live which will get eliminated
- **constant failure rate** → getting problems but not at the high rate like initially
- **wear out failures** → with worse [[maintenance]] / not following [[Lehman's Laws]] , not following [[Clean Code]] practices , more bugs creep in as system decays. have to determine whether system is kept or scrapped

Distinction of early failures, random failures, and wear out failures (which are a different type compared to infant mortality stage) [[Bugs, errors, and faults]]

### Different types of bathtubs 
Using the standard bathtub curve, we can observed whether real failure rates are in line with expected failure rates - if real rates are higher it suggest a flawed development or requirements definition.

how can the system affect the shape of its bathtub curve 
- time axis is not specified, and the curve will change depending on the exact system
- shows whether the system is has [[Good Design]] or poor design. 

what is the bathtub curve for a poor system
- **narrow bathtub** → 
	- high number of problems at the start 
	- problems are gotten rid of quickly, 
	- period of stability is short 
	- problems arise again quickly = quicker quality decline
	- seeing a narrow bathtub can indicate [[Death March]] territory as the team continues to ride the high error ride and a poor system may also take longer to reach the stability period (unsymmetrical bathtub curve)

what is the bathtub curve for a good (ideal) system 
- **shallow bathtub** → 
	 - a few problems at the start 
	- reaches constant failure rate quickly 
	- has long stability of constant failure rate, 
	- rise in problems is shallow with low signs of wear, [[Degrading]] of system quality is slow but unavoidable

### References
 [https://www.modernanalyst.com/Careers/InterviewQuestions/tabid/128/ID/6092/What-is-a-Bathtub-Curve-and-How-Can-it-Be-Useful.aspx](https://www.modernanalyst.com/Careers/InterviewQuestions/tabid/128/ID/6092/What-is-a-Bathtub-Curve-and-How-Can-it-Be-Useful.aspx)

#L1_SoftwareMaintenanceEvolution 