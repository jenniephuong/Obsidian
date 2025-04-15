why should we search code for faults
- faults can be time sensitive so need to be found quickly e.g. BA system problems or ATM crashes
- some failures are more important than others
- some faults introduce security vulnerabilities

historical data can be used to predict where future bugs will tend to be and try to prevent them
- [[Refactoring|preventative refactoring]]

why is accurate prediction of fault-prone code important
- can direct test efforts
- reduces costs
- improves quality

what are the causes of faults
1. requirements were wrong
2. deviation from the requirements
3. logical errors in coding
4. testing inadequacies

what is the ‘requirements were wrong’ fault cause
- might technically ‘work’ but not fulfilling it’s business purpose
- considered the root cause of software faults consisting of
    - **incorrect** definitions e.g. incorrect formulas
    - **incomplete** definitions e.g. unclear or implied requirements
    - **missing** definitions
- more costly [[Maintenance|maintenance]] to correct this fault at production stage compared to early stage

what is the ‘deviation from requirements’ fault cause
- a deliberate deviation from the software requirements including
    - developer **reuses** previous or similar work to save time e.g. Ariane 5
    - developer **omits** functionality due to time / budget pressures
        - by the time system testing uncovers this it will be too late
    - developer **adds** unapproved enhancements
        - too much [[Refactoring|refactoring]] leads to over-engineered code

what is the ‘logical coding errors’ fault cause
- various logical errors including
    - **arithmetic** e.g. division by 0
    - **control** e.g. infinite loop
    - **resource** e.g. buffer overflow and security violations
    - **interface** e.g. incompatible subsystems where one system fails trying to talk to another system - banking systems

what is the ‘testing inadequacies’ fault cause
- shortcomings of the testing process as a result of
    - development process being **cut short**
    - **incomplete test plans** e.g. no boundary conditions, parts of applications not tested at all or properly, poor [[Testing Coverage|testing coverage]] e.g. path / branch testing

what can we use to measure the amount of faults in a system
- [[Fault Density]]

what laws apply to fault proneness
- [[Linus' Law]]
- [[Gall's Law]]


#L5_FaultProneness 