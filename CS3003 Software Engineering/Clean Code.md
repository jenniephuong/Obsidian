what is clean → code code that is
- **elegant** and pleasing to read
- **focused** where each function and class exposes a single minded attitude that remains undistracted by surrounding details [[Single Responsibility Principle (SRP)|[SRP]]]
- **taken care of** by curators, developers made it simple and orderly
- **contains no duplication**, the number of entities (classes and methods) are minimised
	- → limit to this, before each class starts becoming a [[Large Class]], needs to still be understandable
	- → follows [[Rule of Three]]
- follows [[Boy Scout Rule]]

the opposite of [[Dirty Code]]

why do we need clean code → clean code means
- better use of time in the long-term
    - short term pain for long term gain by reducing [[Tech Debt]]
    - saves money as developer’s time is costly to pay for
- easier ramp-up of new staff
    - ramp-up refers to getting new team members up to speed on the system
- easier debugging
- improves maintenance in the long term
    - [[Code Smells]], [[Degrading]], [[Bathtub Curve]], [[Lehman's Laws]] are all impacted by how clean the code is 
- [[Fault Proneness]] reduction
- vulnerability reduction → customer prosecution possible for not updating code to resolve this

what are the consequences of unclean code
- more time understanding the code than actually improving it through [[Refactoring]]
![[Pasted image 20241120092305.png]]
- measuring the productivity of a developer is very difficult e.g. LOC not good metric to measure as comments can count

### rules and factors impacting clean code

what are the general rules for clean code
- follow common sense principles
    - [[KISS]]
    - don’t let [[Tech Debt]] accumulate
    - [[YAGNI]]

what factors impact clean code
- [[Naming Conventions]]
- [[Method Conventions]]
- [[Comments]]
- [[Formatting Style]]
- [[Open Closed Principle]]

purpose of clean code is to ensure [[Legacy Systems]] are maintained as well and for as long as possible

relates to [[Pareto Rule]] 
- getting quality to 100% with clean code principles takes a lot longer, more time, flattened out, 20% extra quality with 80% of the time 
- almost impossible to get clean code 100%, quick gains ![[Pasted image 20241120104642.png]]

what are 2 relevant laws of code cleanliness
- [[Hofstadter’s Law]]
- [[Eagleson’s Law]]


#L7_CleanCode 