> Calculated complexity based on the control flow graph and heavily dependant on decisions (diamonds) and branch nodes
> 
> for a single method P
> CCP(method P) = (# edges - # nodes) + 2

- Commonly used by industry and in lots of tools
- Very useful for identifying white box test cases
- higher number = higher complexity, can decide a threshold complexity value to determine what number is considered ‘too high’ relevant to other method’s CCs

![[Pasted image 20241104104738.png]]

what is the relation between CC and decision diamonds
- modules with no conditionals have a CC of 1, regardless of how long it is
- more diamonds = higher CC

advantages of Cyclomatic Complexity
- It can be used as a quality metric, given the relative complexity of various designs.
- It is able to compute faster than [**Halstead’s metrics**](https://www.geeksforgeeks.org/software-engineering-halsteads-software-metrics).
- It is used to measure the minimum effort and best areas of concentration for testing.
- It is able to guide the testing process.
- It is easy to apply

disadvantages of Cyclomatic Complexity
- It is the measure of the program’s control complexity and not the data complexity.
- In this, nested conditional structures are harder to understand than non-nested structures.
- In the case of simple comparisons and decision structures, it may give a misleading figure.



#L2_SoftwareMetrics 
### References
https://www.geeksforgeeks.org/cyclomatic-complexity/
