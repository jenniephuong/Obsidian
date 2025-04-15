
example looking from the PDP side 
![[Pasted image 20250415130022.png]]

request goes to PEP first 
then it goes to PDP to decide whether to grant or not, based on the PAP and PIP
- PIP - ACL defined here 
- PAP - 


another example looking from the user side
![[Pasted image 20250415130425.png]]

- bob, the application user, makes a request on that application to access 3 data points, that gets sent to PEP
- PEP sends to PDP
- the PDP decided which data points to access or deny and sends back to PEP 
- PEP retrieves data from database and sends it to the application
- bob can now see the requested data points


example where bob wants to modify input parameters to access specific resources from the database
![[Pasted image 20250415130744.png]]


![[Pasted image 20250415130834.png]]