>Public Key Infrastructure - asymmetric encryption with two mathetatically linked keys -
> public and private key

what are the elements of PKI
- Public key - messages can only be decrypted by private key, everyone who needs to access the resource has access to this key
- Private key - decrypts messages (encrypted by matching public key), only known to the person it belongs to (sender)
- Certificate Authority - cert owner (workflow), although client generates public private key pairs
- Trusted Root CA, Cert Revocation Lists, Cert Store, Hardware Security Module

what is a digital signature 
- technique using PKI to authenticate a message - ensure integrity
	- preventing forgery and tampering, impersonation 
- the uniqueness of the digital signature prevents the owner of the signature from disowning the signature, supporting non-repudiation

what is a digest 
 - a hash of the data being signed, aka. the digital fingerprint


how is PKI used for digital signatures 
- ![[Pasted image 20250416125920.png|600]]
1. the message is hashed into a digest
2. the digest is encrypted using the senders private key (authenticity and integrity)
3. the original message and digital signature are sent to the receiver
4. the receiver hashes he original message into a digest 
5. the receiver decrypts the encrypted digest using the public key
6. now the receiver has 2 digests 
	1. compare the digest and if they match, the message is verified 
	2. this confirms authentic (came from sender), [[Integrity]] (not altered), and [[Non-repudiation]] (sender can't deny that they sent it)


what are PKI use cases 
- used in banking and email use cases (digital signatures)
![[Pasted image 20250416125539.png|600]]