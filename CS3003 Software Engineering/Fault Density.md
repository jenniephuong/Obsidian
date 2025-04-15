> a [[Metrics|metric]] that measures the fault count/size of the release

how do you calculate fault density
- number of faults / [[LOC]]![[Pasted image 20241113093326.png]]
	- 2.8% chance of a fault in a line of code 

does a low fault density imply higher quality code
- not always, there are many factors which impact the fault density
- fault density close to 0 is good, but doesn’t always mean the code itself is good

what factors impact fault density
- **Tester Skill:** A highly skilled tester will be more likely to find more faults (and faults of higher quality) than a lower skilled tester - [[Testing Coverage]]
- **Time Spent Testing:** fault density doesn’t take into account the amount of time spent testing. It simply takes a snapshot of time and states “this is how many faults are in the software for this area/lines of code at this time”
- **Fault Type:** Something that fault density doesn't take in to account is different bug types: trivial, minor, major, critical, showstopper etc.
    - If I have a product that has four minor faults, versus a product with two major faults, which product has the lower quality?



#L5_FaultProneness 