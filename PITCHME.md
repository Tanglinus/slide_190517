### [Review] Dynamic Embeddings for Language Evolution (M. Rudolph & D. Blei, 2018)
@snap[south-east]
##### TANG, Linyuan
##### 2019.05.17
@snapend
---
@snap[west span-100]
#### Dynamic Embeddings
- build on _exponential family embeddings_
- [PURPOSE] capture how the meanings of words change over time
- [RESULT] dynamic embeddings provide better fits than classical embeddings and capture interesting patterns about how language changes
@snapend
---
@snap[west span-100]
#### Exponential Family Embeddings (M. Rudolph et al., 2016)
@ul[](false)
- cast word embeddings in a probabilistic framework
@ulend
@snapend
---
@snap[west span-100]
### Datasets
@ul[](false)
- the U.S. Senate speeches from 1858 to 2009
- the history of computer science ACM abstracts from 1951 to 2014
- machine learning papers on the ArXiv from 2007 to 2015
@ulend
@snapend
---
@snap[west span-100]
### related work
There have been several lines of research around capturing semantic shifts.
@ul[](false)
- use features such as POS tags and entropy
- employ latent semantic analysis and temporal semantic indexing
- train a separate embedding for each time slice of the data
  - initialization
  - ad-hoc alignment techniques to stitch them together
@ulend
In contrast, the representations in this work for dynamic embeddings are sequential latent variables.
@snapend
---
@snap[west span-100]
@snapend
---
@snap[west span-100]
@snapend
