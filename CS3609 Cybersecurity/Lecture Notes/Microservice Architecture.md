>each element of the functionally is in a separate service, which scales by distributing the services across servers and replicating as needed
>
>![[Pasted image 20250415185019.png|300]]

better than [[Monolithic Architecture]]
- if one part of the system is accessed, other parts can still be protected since they are separated

however, still susceptible to the following attacks 
- [[Social Engineering]]
- [[Injection]]
- [[Patches]]


e.g. Amazon has a composite UI where each component of the interface is managed by a microservice, making it difficult to [[Monitoring]]
![[Pasted image 20250416094204.png|600]]