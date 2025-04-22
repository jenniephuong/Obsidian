>a network security tool that monitors ***network traffic*** and ***devices*** for known malicious activity, suspicious activity or security policy violations.

what is intrusion detection
- a device or piece of software that monitors networks for malicious activity, policy violations or unwanted ‘intrusions’.

why are IDS needed
- criminals entering a system had a certain signature, sign of something suspicious
- systems on a network are vulnerable to attack as data is sent across the network 
- used as an addition to a firewall as embedded attacks might be allowed by the firewall

![[Pasted image 20250416095623.png]]

what are the two types of IDS
- [[Host-based IDS]]
- [[Network IDS]]
- organisations usually use a combination of the two, in conjunction with firewalls

what is a network signature 
- represents a pattern that is a component of a known attack

what's the difference between IDS and Firewall
- firewall controls traffic based on a set of defined rules e.g. IP addresses, ports, protocols - allowing or denying traffic between the computer and offer systems
- IDS actively monitor traffic and use pattern recognition to identify suspicious activities by comparing the activities against a database of known threats 

what detection method do IDS use for analysis 
- pattern/[[Signature-based]] IDS 
- [[Anomaly-based ]]IDS
- rules for [[Internet Control Message Protocol (ICMP)]] packets can be created 


this is a markov based attack detection method, but I'm not gonna focus too much on it since it's a bonus paper than the lecturer recommended
![[Pasted image 20250422104725.png|600]]