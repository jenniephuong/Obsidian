IoT devices are physical hardware like sensors, appliances, machines, that connect to the internet - they are often built with functionality in mind so security is neglected  

how are vulnerabilities introduced in mobile and IoT systems / applications
- not patched regularly
- use public internet with unencrypted data stream
- poorly developed to introduce dependencies and default credentials 
- outdated firmware with exploits 
- bad code (explained further down)

![[Pasted image 20250415182242.png|500]]

however, security measures can be embedded into the devices
devices can have built in mechanisms to ensure only authorised 

during the development of the code of mobile applications, secure protocols can be used to ensure there is secure communication and storage e.g. 
- https - secure web communication
- context.MODE_PRIVATE - ensure file created is available only to the application and private to everything else
- ![[Pasted image 20250415183017.png|600]]

another example is app.run(debug=true)
- in development it's used for debugging but if used in production it can expose information about file paths, code structure, and configurations in it's error messages that can be exploited
- ensure debug = false 
![[Pasted image 20250415183408.png]]

another example in PhP - bad code can lead to SQL [[Injection]]s 

![[Pasted image 20250415183811.png|600]]