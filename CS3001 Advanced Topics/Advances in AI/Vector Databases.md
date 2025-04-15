https://www.datacamp.com/blog/the-top-5-vector-databases

A specific type of database that stores multi-dimensional data points instead of scalar values, the vectors represent data in numerous dimensions 
- number of dimensions vary from few to thousands
- quickly and precisely locate data based on vector proximity or resemblance 
- searches don't just rely on exact matches but can match based on semantic or contextual relevance 

this content store can be open (internet) or closed (classified documents) depending on the need.

how to query a vector database 
- work by using measures of similarity to find the closest matches - APP, Approximate Nearest Neighbour 

examples 
- Chroma 
- Pinecone
- Weaviate
- Faiss
- Qdrant
- Milvus
- PGVector

how to create a vector database 
- need to create [[Embeddings]] for unstructured data, allows us to use all media types including images, text, audio, into the vector database 
- neural networks can be used to convert the text / data chunk into a numerical embedding 

![[Pasted image 20250224185512.png]]

pros of vector databases 
- scalability and adaptability - as data grows it can scale across multiple nodes, the system can be tuned to include any new data as needed 
- multi-user support and data privacy - data isolation 