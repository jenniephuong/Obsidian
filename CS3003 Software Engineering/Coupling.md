> The degree of independence between classes, the amount of interactions/ dependencies among classes - looking externally to the class

The number of dependencies is directly proportional to the amount of coupling

Factors that increase coupling between class A and class B include
- A has an attribute that refers / of type B
- A call on a method from B
- A is a subclass of B

Variables involved with coupling include 
- **degree** - num of connections should be small
- **ease** - there should be obvious connections between coupled modules without needing to understand implementation of other unnecessary modules
- **flexibility** - modules should be interchangeable so that can be removed or improved in the future

![[Pasted image 20241104224643.png]]

Relates to the [[Law of Demeter (LoD)]]

what are the different coupling types from mid to worst
- [[Uncoupled]]
- [[Stamp coupling]]
- [[Common coupling]]
- [[Content coupling]]

what are the consequences of high coupling
- classes difficult to understand in isolation
- more sensitive to change as changes in one class ripple to others, making [[Maintenance]] harder 
- classes are hard to reuse as they need to include all coupled classes
- due to interdependent modules, takes more time or effort to test or assemble, and more [[Bugs, errors, and faults|bugs]] could appear and remain

what are the consequences of low / not enough coupling
- can mean poor cohesion
- poor code understandability making maintenance difficult
- can impact the functionality of the system

Coupling needs to be minimised as much as possible, and still ensures efficient system functionality -  threshold coupling
[[Refactoring]] aims to find the optimal level of coupling, and reduce the unnecessary existing coupling 

### References
[https://ducmanhphan.github.io/2019-03-23-Coupling-and-Cohension-in-OOP/](https://ducmanhphan.github.io/2019-03-23-Coupling-and-Cohension-in-OOP/)
https://wiki.c2.com/?CouplingAndCohesion
[https://martinfowler.com/ieeeSoftware/coupling.pdf](https://martinfowler.com/ieeeSoftware/coupling.pdf)


#L4_SoftwareComplexity 