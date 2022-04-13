# Distributed semantic representations
In this project I expirement with distributed semantic representations using Word2vec, Glove50d and Glove100d implementations

- Dense distributed representations represent words as embeddings in a continuous vector space where semantically similar words are mapped to nearby points.
- in the following notebooks i test word2vec, Glove50d and Glive100d embeddings on 4 different analogy tests to measure to what extent are embedding models able to capture semantic relationships(and surplrisingly more!) between words.
- The goal of the analogy tests is to predict the 4th entry in a row given the analogy expressed by the first 3 words.

# Analogy tests:
### Test on plural-verbs analogy Ex:
[['decrease', 'decreases', 'describe', 'describes'],  
['decrease', 'decreases', 'eat', 'eats'],  
['decrease', 'decreases', 'enhance', 'enhances'],  
['decrease', 'decreases', 'estimate', 'estimates']]

### Test on plural-nouns analogy Ex:
[['banana', 'bananas', 'bird', 'birds'],  
['banana', 'bananas', 'bottle', 'bottles'],  
['banana', 'bananas', 'building', 'buildings'],  
['banana', 'bananas', 'car', 'cars']]

### Test on capital_common_countries analogy Ex:
[['Athens', 'Greece', 'Baghdad', 'Iraq'],  
['Athens', 'Greece', 'Bangkok', 'Thailand'],  
['Athens', 'Greece', 'Beijing', 'China'],  
['Athens', 'Greece', 'Berlin', 'Germany']]

### Test on currency analogy analogy Ex:
[['Algeria', 'dinar', 'Angola', 'kwanza'],  
['Algeria', 'dinar', 'Argentina', 'peso'],  
['Algeria', 'dinar', 'Armenia', 'dram'],  
['Algeria', 'dinar', 'Brazil', 'real']]
 
# Results:
The following numbers represent accuracy wheras accuracy is calculated as correctly answered / number of examples on each analogy test.
| Model \ analogy test | plural verbs| plural nouns | capital common countries | currency |
| --- | --- | --- | --- | --- |
| Glove50d | 0.35 | 0.60 | 0.80 | 0.08 |
| Glove100d | 0.58 | 0.71 | 0.93 | 0.14 |
| word2vec | 0.68 | 0.89 | 0.83 | 0.35 |


![download (3)](https://user-images.githubusercontent.com/87248009/163086976-bd6b28bf-0160-41f3-9535-046685b9444b.png)
