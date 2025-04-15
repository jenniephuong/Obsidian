> How much are the responsibilities in a class related, the degree to which all methods in the class are 'directed towards a single task'.

Looks at inter-module relationships
- **no cohesion** means classes should probably be split up
- **low cohesions** increases complexity and likelihood of [[Bugs, errors, and faults|bugs]]

what should developers aim for with cohesion
- **high cohesion** - to structure methods in a class so that all methods are related and essential to performing the same task

what are the different cohesion types from best to worst
- [[Functional cohesion]]
- [[Sequential cohesion]]
- [[Temporal cohesion]]
- [[Coincidental cohesion]]

(Low) Cohesion usually results in a [[Large Class]] since developers just add loads of functionality into the class.
Low cohesion can be cause by [[Tech Debt]], as the debt piles up since the developers didn't take the time to separate the class 

[[Design Patterns]] are meant to lead to cohesive classes but can actually make cohesion worse 
- become a repo for random methods that don’t fit in other places - when a method or part of a system doesn’t fit into the design pattern, it becomes more incohesive since they are forced to fit somewhere they don’t belong, might have been better not to use one where there’s more flexibility

### References
[https://ducmanhphan.github.io/2019-03-23-Coupling-and-Cohension-in-OOP/](https://ducmanhphan.github.io/2019-03-23-Coupling-and-Cohension-in-OOP/)
https://wiki.c2.com/?CouplingAndCohesion

#L4_SoftwareComplexity 