> the level of a class in the inheritance tree
> the deeper the class is the more methods and variables it inherits making it more complex

Inheritance based complexity metric 
- inheritance should be used to maintain complexity - not increase it

what does the amount of DIT show 
- high DIT can increase faults but not direct correlation 
- middle depth classes are usually most fault prone as they are consulted less than root or deep classes

how does DIT impact reusability 
- deep trees are good though since it promotes method reuse

are high depth or lower depth classes better to change
- M - changes can trickle down to sub classes
- r - possibly easier to localise changes, but needs to consider more inherited methods and attributes

![[Pasted image 20241104105313.png]]


#L2_SoftwareMetrics 