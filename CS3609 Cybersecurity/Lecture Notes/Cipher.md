>an algorithm to perform encryption or decryption

a cipher is unconditionally secure if no amount of ciphertext will give enough information to yeild a unique plaintext, however given enough time and resources almost any cipher can be broken
- the cipher needs to be difficult enough that it is computationally infeasible to break

what are the types of ciphers
- block cipher
- stream cipher
- transposition cipher
- substitution cipher

different ciphers should be used depending on the type of data to encrypt 

what is a block cipher
- encrypts blocks of data at a time, turning them into fixed-size ciphertext blocks, decryption also occurs one block at a time
- used for large file encryption like databases 
  ![[Pasted image 20250416112720.png|600]]

what is a stream cipher
- encrypts messages in a continuous stream one bit of data at a time
- used for video encryption
  ![[Pasted image 20250416112751.png|600]]

what is a transposition cipher 
- rearranges characters in the plaintext without altering the letters themselves
- done by arranging the character into rows and reading down the columns
  ![[Pasted image 20250416112759.png|600]]

what is a substitution cipher
- replace each character in the plaintext with a new ciphertext character by using a key (function)  
- e.g. Caesar cipher 
  ![[Pasted image 20250416112811.png|600]]