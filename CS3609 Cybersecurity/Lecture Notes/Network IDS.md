>monitor inbound and outbound traffic to devices across the network

where can they be placed 
-  can have both an external (outside firewall) and internal (inside firewall) NIDS connected to a switch or a hub
	- external - shows attacks that the firewall faces 
	- internal - identify attacks that bypass the firewall, catch insider threats or hijacked user accounts
- usually placed 'out-of-bounds' so that traffic doesn't directly pass through where NIDs can disrupt legitimate traffic, but it analyses copies of network packets to flag traffic

what can NIDs do
- can change rules to filter traffic and stop the attack

![[Pasted image 20250416100206.png]]

e.g. SNORT - an open source NIDs system 

![[Pasted image 20250416101824.png|600]]