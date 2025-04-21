>the process of breaking encrypted messages to discover their meaning

what are the types of cryptanalysis attacks 
- ciphertext only attack
- known-plaintext attack
- chosen-plaintext attack
- chosen-ciphertext attack

these attacks usually carried out when the attacker already has access to the system


what is a ciphertext only attack
- cryptanalyst has access to only a segment of encrypted data  
- have to use patterns in the ciphertext to determine the plaintext 

what is a known-plaintext attack
- cryptanalyst had access to some plaintext and ciphertext 
- e.g. if there is a code that is always given before the password![[Pasted image 20250416115405.png|500]]

what is a chosen-plaintext attack
- the attacker can convert chosen plaintext into ciphertext and observe the output, giving them more flexibility and insight into the encryption method 

what is a chosen-ciphertext attack
- only relevant in asymmetric key systems and hash functions
- attacker submits data with same cipher and key that they are trying to break, to the decryption device
	- this lets them see if the plaintext is returned or if something else is returned, allowing them to learn the effect that the d