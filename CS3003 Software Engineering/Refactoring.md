> the process of changing a software system in such a way that it does not alter the external behaviour of the code, yet improves its internal structure

Can be done at any time but most useful during the end of the [[Bathtub Curve]] where a system is reaching the end of it’s lifecycle where it starts to show signs of [[Degrading|decay]].

Fenton & Neil’s results
- within a system - ‘small number of modules contain most of the [[Bugs, errors, and faults|faults]]’
- links to [[Pareto Rule]] 
- if we know this, we can direct effort to refactoring the 20%

does refactoring change system behaviour
- no, the user should not notice any difference

Refactoring a system aims to make the system follow the [[Software Engineering Laws]]

what type of [[Maintenance]] is refactoring
- **preventative** (prevent [[Tech Debt]], making things better now to prevent them debting up)
- **perfective** (improve existing codebase)

what type of project lifecycles use refactoring
- especially important in XP and TDD
- constant regression testing important

what is the aim of successful refactoring
- modify the existing codebase to
    - remove duplicate code - need to change in every area it’s duplicated
    - improve [[Cohesion]] and reduce [[Coupling]]
    - improve understandability and maintainability

when should you refactor
- Fowler - refactor consistently and mercilessly
- when you recognise a warning sign like [[Code Smells]]
- when you have to fix a [[Bugs, errors, and faults|bug]] since after the bug fix the affected code around it can be refactored
- when you do a code review as part of a pair or [[Mob Programming]]

what tools can you use for refactoring
- eclipse, netbeans, refactor tools build into the IDE

what are the methods of refactoring (fowler suggest 72)
- [[Extract Method]]
- [[Extract Class]]
- [[Extract Subclass]]
- [[Move Method]]
- [[Move Field]]
- [[Encapsulate Field]]
- [[Replace Magic Number With Symbolic Constant]]
- [[Remove Dead Code]]
- [[Consolidate Duplicate Conditional Fragments]]
- [[Substitute Algorithm]]

what are the advantages of refactoring
- Reduces duplicate and inefficient code
- Improve cohesion, reduce coupling (unnecessary coupling)
- Improves the understandability of code, maintainability, etc. by reducing complexity
- Can help reduce technical debt
- Can help reduce bugs since the code is more maintainable
- Can be done at any stage of a system’s life

what are the disadvantages of refactoring
- Opportunity cost - there are many other things that can be done instead of refactoring and this might be time better spent
- Complex in many cases and always needs significant re-testing (no free lunch)
- No guarantee that the refactoring won’t break despite testing or that it makes code any less bug-prone
- Time – it takes time to do refactoring and communication overhead if you’re working in a team
- There is not a huge amount of evidence that refactoring actually provides the benefits it claims
- Does it make future maintenance easier?
- Can lead to developers going down “rabbit holes”
- Companies punish developers (no promotion) for refactoring compared to developing new features

### References
[codeproject.com/Articles/771894/When-Refactoring-Is-A-Bad-Idea](http://codeproject.com/Articles/771894/When-Refactoring-Is-A-Bad-Idea)


#L3_SoftwareRefactoring 