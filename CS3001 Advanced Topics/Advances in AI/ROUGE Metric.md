>the F1 score (overlap) for N-gram precision and recall

n-gram = sequence of N words
- e.g. can be ROUGE-1 or ROUGE-2 for N word sequences
```
##for unigrams it is  
(I),(love),(Machine),(Learning)  
##for bigrams it is  
(I love),(love Machine),(Machine Learning)
```


recall = quality of accurate n-grams
- num of overlapping n-grams / number of n-grams in reference

precision = quality of n-grams in the model output 
- num of overlapping n-grams / number of n-grams in output text

ROUGE-score = (2 * (precision * recall)) / (recall + precision)
over 0/5 is considered good 