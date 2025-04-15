>puts all of the application functionality into a single process, and scales by replicating the monolith on multiple servers

![[Pasted image 20250415184928.png|300]]

what are the vulnerabilities 
- a change made to the small part of the application required the entire monolith to be rebuilt or deployed making it harder to maintain the structure 
- therefore an attacker gaining access to one part of the system allows them to gain access to the entire system

what attacks are monolithic architecture prone to 
- [[Social Engineering]]
- [[Injection]]
- not having updated [[Patches]] 

