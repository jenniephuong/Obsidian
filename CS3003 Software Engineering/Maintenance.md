> the process of modifying a software system or component to correct [[Bugs, errors, and faults]], improve performance or other attributes, or adapt to a changed environment

what are the types of maintenance
- **Adaptive maintenance** → adapting to changes in the environment (both hardware and software changes e.g. responding to tax laws / ISA changes at DHA)
- **Corrective maintenance** → correcting and bugs and preventing failures
- **Perfective maintenance** → making the existing code better (refactoring - not only for when bugs exist)
- **Preventative maintenance** → future proofing code for later (only possible when you get time, the others are done during regular maintenance work)

[[Refactoring]] is a maintenance technique

what are the limitations of maintenance
- expensive
- difficult

why is maintenance expensive (stats)
- Sommerville reports 70% software costs is due to maintenance
- Costs **vary** across application domain (e.g. real time, embedded, games)
- Classic example: US air force project: £20 per line code to develop and £2,500 per line code to maintain (expensive regression testing)

why is maintenance difficult (stats)
- 47% effort goes into understanding the system and identifying **dependencies** (Pfleeger)
- Making changes is also **risky** because of **ripple effects** and dependencies
- Can be a low morale job

what factors affect maintenance and [[Evolution]]
- **Team stability** → people leaving the team means information they hold might leave too, less people to contribute - high dev churn, developers going in and out of the project overall get a surface level understanding
- **Poor development practice (quality)** → subjective quality, but worse quality metrics (e.g. time complexity, [[Cohesion]], [[Code Smells]], bug infested) are harder to maintain and evolves worse
- **Staff skills** - low skills means lower quality maintenance
- **Program age and structure** - old legacy code is more brittle and easily degraded
- **[[Tech Debt]]** - leaving tech debt means more time and effort to make the change when it would have been less complex to make from the beginning since code decays and gets worse over time

what are the 6 topics relevant to maintenance (and hence system evolution)
- [[Software Evolution Theory]]
- [[Mob Programming]]
- [[Bathtub Curve]]
- [[Brooks' Law]]
- [[Death March]]
- [[Pareto Rule]]

#L1_SoftwareMaintenanceEvolution 