> framework used to enforce access controls using an abstract *'reference monitor object'* that operates at the boundary between the user and the object (meaning no direct subject interaction with the object), validating the access to objects. (like a bouncer at a club)

![[Pasted image 20250415120454.png]]
e.g., a student trying to access a coursework document

what are the properties of the reference monitor 
- cannot be bypassed
- controls all access
- cannot be altered or modified 
- can be verified and tested to be correct 

what is the subject 
- the person trying to request access to the object 

what is the audit log 
- keeps track of every detail of activity between the subject and reference monitor 
- e.g. apache log 
  ![[Pasted image 20250415154933.png|]]

what is the security kernel database 
- e.g. access control list 
- stores the policies and access control rules that the reference monitor can reference

how does the reference monitor model work 
- subject makes the request for access and is identified 
- reference monitor logs the subject making request the object, with the timestamp and all other metadata 
- reference monitor confirms whether the subjects exist in the SKD and whether they have the correct privileges to carry out the request they have made
- reference monitor allows or denies access

[[AAA Servers]] are practical implementations of the reference monitor model that focus on centralising the 3 As.