> Adding human resources to a late project makes it later

![[Pasted image 20241104101947.png]]
the widening gap shows more people = less productive individuals

Brooks' Law is based on...
- **Ramp up** →
	- takes time and resources to train new staff on what’s happening with the project
	- existing productive staff lose productivity by training newbies, and facilitating more communication than previous 
	- new hire mistakes that set the project back
- **Complexity of communication** → 
	- each additional person brings a fixed number of additional hours (40), growing linearly with each person, but the number of communication paths and time and effort of coordination overhead grows more rapidly and consume the available hours - resulting in a net loss
	- more opportunity for communication error compared to few people
	- e.g. teams calendar with 100 billion sync meetings, reporting events, scrum of scrums
- **Software Structure** →
	- software projects have a point where work cannot be broken into smaller, independent pieces *without resulting in higher costs*, meaning even new trained individuals doesn't mean they could make progress on the project

Coordination and ramp up costs often invisible, making it easy to ignore when wanting to add new people. 

If brooks laws is applied, it’s essentially following the [[Death March]] trajectory

### Is Brooks' Law the only cause?
Brook’s law not the only reason for project decline e.g. [[Tech Debt]], onboarding costs (correct number of developers but long time to onboard them properly)

Saying that Brook’s law makes projects later is hard to validate as we can’t know what would have happened if new hires hadn’t been added to the project - the project timeline estimates (even before new hires added) can be invalid themselves (not all time estimates are well-founded, often optimistic)
    - Standish Group’s Chaos report found that the average business systems project overran its original schedule by 120 percent
- amount of effort lost to training must exceed productivity of new hires when they’re finally productive
- Also, is it Brook’s law, or is it just poor project management?
    - Brook’s law implies that it only applies during final stages of a project (e.g. NASA projects recommends small senior staff first, then adding more once requirements + architecture defined) - but how do we know when the final stages are?
    - Poor project tracking - no clarity on what % of the project is finished means people think they’re at risk of Brook’s law earlier than they really are e.g. if a project think’s they’re 90% done, don’t want to risk new hires, turns out they’re only 30% done, and adding new people would have been better, but they left it too late and have to add new people anyway
    - or poor project tracking gives the illusion that there’s enough time for the new hires to be productive despite the raining time
    - or poor project management = poor documentation, making ramp up time longer than necessary meaning adding people later on with less risk

### References
[https://codescene.com/blog/visualize-brooks-law/](https://codescene.com/blog/visualize-brooks-law/)
[https://stevemcconnell.com/articles/brooks-law-repealed/](https://stevemcconnell.com/articles/brooks-law-repealed/)


#L1_SoftwareMaintenanceEvolution 