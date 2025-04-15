#core

A weakness that leaves you exposed to a threat, can cause legal liabilities and software vendors need to protect themselves from their own liabilities

> Vulnerabilities exist within [[Assets]]
> Vulnerabilities increase the likelihood of [[Risk]]

___

what different vulnerabilities are there in a system
- technology weakness
- configuration weakness
- security policy weakness

what are technology weaknesses
- primarily protocol weaknesses that exist in the design in the protocol making them very hard to change since protocols are dependant on each other
- TCP/IP protocol, HTTP, FTP, ICMP, ARP
- Software vulnerabilities (see SSDF for reference)
    - common - deficiently in the software code itself e.g. buffer overflow as a result of poor memory management

what are configuration weaknesses
- the system / software is not set up properly which creates more weaknesses e.g.
- weak or default passwords
- misconfigured firewall
- leaving ports open

what are security policy weaknesses
- weak security policy or policy enforcement or implementation
- software and hardware installations and changes not following policy
- lack of 2 factor authentication

how are vulnerabilities specified after a security researcher identifies it
- using [[CVE]] framework
    - notify the vendor of the software / protocol / device so they can fix it
    - assign the vulnerability to a unique CVE identifier
    - patches refer to the CVE and once fix has been made and not before, the vulnerability is announced (e.g. sims 4 patch notes)