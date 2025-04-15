what is the difference between software metric vs. software measurement
- measurement - the process of measuring
- metric - the result of measuring

what does software measurement help us do
- **to understand** → makes current activity visible and helps us establish guidelines like methods / classes too long
- **allows us to control** → predicts outcomes and change processes e.g. AI techniques to predict future behaviour based on past metrics
- **encourages us improve** → when we measure our product we can establish quality targets and aim to improve

link between maintenance + evolution and software metrics
- we can understand why the system has that [[Bathtub Curve]] using software metrics, better understand the system and why it’s happening e.g. what metrics does a system with  a good shallow Bathtub Curve (long stability) show?
- helps us target [[Maintenance]] where needed in the system and make decisions on what to do to maintain the system

are metrics always good
- metrics can also be taken to the extreme - following them so rigidly that they act as limitations rather than guidelines
- metrics are only useful in comparison to other system metrics, e.g. a single measurement is useless unless we understand what the threshold is for a 'high' or 'low' value

what can metrics measure
- [[Software Size]]
- [[Software Structure]]
- OOP complexity using [[OOP Metrics]]

what are the challenges of using metrics
- professionals may show over-optimism and over-confidence in metrics
- metrics can cause more harm than good - data is shown because its easy to gather and display rather than actually have useful interpretations and just wasting everyone’s time
- metrics may have a negative effect on developer productivity and well being - used to rank employees
- academic / industry divide - different places have different options on which metrics are useful e.g. industry wanting easy simple metrics, or industry more interested in code churn (amount of how much code changes in the codebase) and level of technical debt

what are the applications of metrics
- making decisions using an audit grid assessing business value and system quality of a system
- for each system, plot them on the audit grid (y axis should be business value)
- ![[Pasted image 20241104110204.png]]

	- discard
	- keep
	- 9+10 [[Refactoring]] and [[Reengineering]] to improve quality (taking time and effort) or keep as is
	- 4+5 get rid of them, or change them to improve the business value (which could impact quality)

#L2_SoftwareMetrics 