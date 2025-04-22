>rule based, detects attacks by compares current traffic with signatures (patterns like a known byte sequence in network traffic, or known intrusion sequence). signatures need to be updated as attackers will change their attacks to go undetected

most commonly used in industry e.g., SIEM, firewall, router, system and event logs

what are the limitations of signature based
- requires high quantity of data 
- generates many false positives → based on if-then sequence, as soon as pattern detected it is flagged, rules written are based on assumptions, so an attack may be incorrectly categorised as an attack
- require frequent updates → new attack patterns requires new rules to be creates
- difficulty in detecting ‘unknowns’ → if the pattern is not already put in the rules, won’t be detected correctly, needs combination with other IDS approach