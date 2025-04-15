systems made up of 
- components 
- interfaces 
- databases 

software is made up of different components which each have a function eg., login, register
the components are linked using interfaces 

interfaces are used to connect software systems

![[Pasted image 20250415181416.png]]

how are security vulnerabilities introduced when connecting the elements 

perhaps you develop a system where all the existing components (create account, login) work as expected even after testing 

however, when trying to connect the components, [[Vulnerabilities]] can be introduced that compromise overall security and regression testing ([[Software Testing]]) and end to end ([[System Testing]]) is required whenever trying to interface new components

the database and application may reside on a different server, so a connection needs to be made between application and database - this link via networks, opens risks of data theft and etc.