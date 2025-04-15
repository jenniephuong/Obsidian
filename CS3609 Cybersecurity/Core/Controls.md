#core

> Controls are used to mitigate [[Risk]]
> Controls are used to mitigate [[Vulnerabilities]]
> Controls are used to mitigate [[Threats]]

___

Any controls and policies implemented need to be anchored to [[CIA Triad]]

#lecture

what is an access control 
- the process of **granting** or **denying** specific requests or attempts to
    - obtain and use information and information processing services
    - enter specific locations
	e.g., requiring an active user ID to access Wiseflow 


what are the 2 items that access controls link together
- subject - who wants to request access 
- object - the thing being requested e.g. database, files, software, network, vehicle, computer, hard drive - anything an organisation works with


how do controls operate within an organisation
1. authenticate the **subject**
2. request the **object** access
3. authorise the request - output is to approve or deny access to the object


what is the operational architecture for organisations to ***DEFINE*** access controls
- controls first need to be defined and then authorised and then implemented
	1. [[Organisational Policy]]
	2. [[Functional Policy]]
	3. [[Mechanisms]]
	   
	   ![[Pasted image 20250415104546.png|550]]


what are the two categories of access controls 
- physical access controls - used to secure physical spaces or objects  e.g., buildings, car parks using **keys**
- logical access controls - used to secure systems or networks e.g. restricting certain users form accessing network resources and performing certain tasks using a **username and password**
	- deciding which users can do what
	- monitoring what a user does in a system
	- stop, restrict, or limit user actions


what are the practical ways access controls can be implemented 
- technical controls - electronic means e.g., login credentials, MFA
- physical controls - lock and key, ID badge, barriers 
- administrative controls - ensuring different people have different access and usage privileges e.g., staff vs. student 


how do organisations ***ENFORCE*** access controls
- using the [[Reference Monitor Model]] (framework)


what are access control policies 
- the specific set of rules that allow specific groups of users perform specific actions on a set of specific resources 


what are the key elements that need to be considered when managing access control policies
- users (subjects) - who wants to use the system e.g., IT admins, students
- resources (objects) - the protected objects in the system that can only be accessed in authorized ways by authorized subjects, e.g., emails
- actions - activities the authorized users can perform of the resources, e.g. delete, add, modify
- relationships - optional permissions granted to an authorized user e.g. read, write, execute
  
  ![[Pasted image 20250415123529.png|400]]

e.g. creating access control policies for a hospital environment
1. users = doctors, staff, patients
2. resources = wards, vending machine, hospital tech
3. actions = use vending machine, enter wards, operate machines
4. relationships = doctors → operate machines, all staff and patients → enter wards
   
   ![[Pasted image 20250415123736.png|500]]


what are examples of access controls for a mobile device
- Multi Factor Authentication MFA - require two or more verification factors to gain access
- Mobile Device Management MDM - control the whole device, what actions can be done e.g. work devices prohibit USB connections
- Mobile Application Management MAM - higher privileges needed for application itself, restrict features of the app 


what are the four key processes of access controls 
- [[Identification]]
- [[Authentication]]
- [[Authorisation]]
- [[Accountability]]


what does centralised access control mean
- an approach where a single common entity (individual/ department/ device) is used to manage who can access the system and network, instead of it being done locally in lots of places. 


how do organisations ***CENTRALISED*** access controls
- using [[AAA Servers]]


how are access controls ***MONITORED*** for different organisations
- manually monitoring requests is okay for small businesses, however for a commercial approach, with thousands of users in an organisations, special software required to monitor access. security score can also be calculated to help to detect issues
	- e.g. Microsoft Defender - traffic into and out of the system are monitored and can pinpoint specific users and their IP addresses, can automatic log out users to protect the environment
  
	  ![[Pasted image 20250415124355.png|550]]


{ but who decides who gets access and who doesn't get access } -> use formal access control models to help decide this

what are formal access control models 
- models / guidelines used to design (not implement) the logic behind who has access to each resource


what are the formal models of access control (confidentiality and integrity)
- [[Discretionary Access Control (DAC)]]
- [[Mandatory Access Control (MAC)]]
- [[Non-discretionary Access Control]]
- [[Role-based Access Control (RBAC)]]
- [[Attribute-based Access Control (ABAC)]]
	these can be used to create the access control list 

formal access control models provide the framework for security policy models to be created to apply to specific environments and to meet specific goals 

what are the different types of security policy models 
- [[Bell-LaPadula Model]]
- [[Biba Model]]
- [[Chinese Wall (Brewer and Nash Model)]]

what is an access control list / matrix (ACL)
- the set of rules that ***explicitly*** states the level of access each subject has to each object, based on a formal access control model
- can be a list or a matrix 
  
  ![[Pasted image 20250415151552.png|300]]![[Pasted image 20250415150939.png|500]]
	- e.g., read, write, execute

	example table headers include...
	- subject | asset -> bob 
	- classification | asset -> top secret 
	- role | asset -> student