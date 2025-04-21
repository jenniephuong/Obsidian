>protects against host-level attacks by monitoring all processes ***inside a host*** (computer)
 

how do HIDs work
- first install on a specific endpoint e.g. server computers and run as software process
- intercept and examine system calls or specific processes to identify dis-allowed behaviour or patterns - by taking period snapshots of critical OS files and comparing them over time
- can perform pre-defined actions e.g., stopping or reporting the infraction

what types of issues can HIDs identify 
- Cryptojacking - when a computer is controlled by a cryptocurrency miner and used to generate cryptocurrency
- inappropriate traffic originating inside the network
- anomalies specific to the host or user e.g., user sending 10x the volume of emails in an hour/ processes trying to use exploits
- [[Network IDS]] might not notice these issues 
- monitoring process disk usage for suspicious usage 
- can catch malicious activity e.g. ransomware, before it spreads to other devices
- log file or configuration manipulation 


e.g. OSSEC is the most widely used HIDs
![[Pasted image 20250416095523.png]]