https://arxiv.org/pdf/1706.03762

A sequence to sequence neural network model with attention

Attention is focused on specific parts of a sequence.
Decoder self-attention is different from encoder self-attention. Encoders receive all tokens at once and see all
tokens in the input sentence.
Decoders generate one token at a time and do not know which tokens will be generated in future.

![[Pasted image 20250421170416.png]]

##### the encoder 
uses word embeddings to convert words to vectors (done using neural networks with weights and activation functions)
- each word may have multiple embeddings

use positional encoding to keep track of word order
- difference between embedding position (the word's order in the sentence) and individual embedding sequence (the embedding order for a single word)
- sine and cosine graphs are used to give positional encoding values to the corresponding order of the word embedding e.g. all first word embedding use 1 sine function
- creates a unique embedding sequence for each word

![[Pasted image 20250421184947.png]]


uses self-attention to maintain the relationship between words 
![[Pasted image 20250421185342.png|500]]
- works by creating query values (based on the positional embeddings) for each word and calculating the similarity between each word is to all of the words in the sentence (key values), including itself, for every word in the sentence - e.g. using dot product

![[Pasted image 20250421185525.png|400]]

the similarities are used to determine how the transformer encodes each word

multi-head attention involves stacking attention cells to capture the relationship among the words

postion values are then added to self-attention values and normlaised

![[Pasted image 20250421190727.png]]

##### the decoder