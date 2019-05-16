### [Review] Dynamic Embeddings for Language Evolution (M. Rudolph & D. Blei, 2018)
@snap[south-east]
##### TANG, Linyuan
##### 2019.05.17
@snapend
---
@snap[west span-100]
#### 1. Introduction
@ul[](false)
- [PURPOSE] dynamic embeddings (D-EMB) analyze documents that span many years, where the way words are used changes over the course of the collection
- [RESULT] D-EMB provide better predictive performance than classical embeddings and capture interesting patterns about how language changes
@ulend
@snapend
---
@snap[west span-100]
#### 1. Introduction
@ul[](false)
- build on *exponential family embeddings*
  - include dynamics into the *Bernoulli embedding model*
- cast the embedding vector as a latent variable that drifts via a Gaussian random walk
- when fit to data, the D-EMB capture how the representation of each word drift from slice to slice (one per year)
@ulend
@snapend
---
![example1](assets/img/img1.png)
---
@snap[west span-100]
#### 1.1 Exponential Family Embeddings (M. Rudolph et al., 2016)
An EFE is a conditional model. It has three ingredients:
@ol[](false)
- the context
- the conditional distribution of each data point
- the parameter sharing structure
@olend
@snapend
---
@snap[west span-100]
### 2. related work
There have been several lines of research around capturing semantic shifts.
@ul[](false)
- use features such as POS tags and entropy; employ latent semantic analysis and temporal semantic indexing
- train a separate embedding for each time slice of the data (initialization or ad-hoc alignment techniques to stitch them together)
@ulend
@snapend
---
@snap[west span-100]
### 2. related work
In contrast, the representations in this work for dynamic embeddings are sequential latent variables.
Two similar models:
![ref1](assets/img/ref1.png)
![ref2](assets/img/ref2.png)
@snapend
---
@snap[west span-100]
### 2. related work
Another area of related work is dynamic topic models.
@ul[](false)
- describe documents in terms of topics, which are distributions over the vocabulary, and then allows the topics to change
- some dynamic topic models also use a Gaussian random walk to capture drift in the underlying language model
@ulend
Topic models capture co-occurrence of words ate the document level and focus on heterogeneity. Word embeddings capture co-occurrence in terms of proximity in the text.
@snapend
---
@snap[west span-100]
### 3. Dynamic embeddings
@snapend
---
@snap[west span-100]
### 3. Dynamic embeddings
@snapend
---
@snap[west span-100]
### 3. Dynamic embeddings
@snapend
---
---?image=assets/img/proc.png&position=right&size=contain
@snap[west span-50]
### 3. Dynamic embeddings
@snapend
---
---?image=assets/img/algo.png&position=right&size=contain
@snap[north-west span-70]
### 3. Dynamic embeddings
@snapend
---
@snap[west span-100]
### 3. Datasets
@ul[](false)
- the U.S. Senate speeches from 1858 to 2009
- the history of computer science ACM abstracts from 1951 to 2014
- machine learning papers on the ArXiv from 2007 to 2015
@ulend
@snapend
---
@snap[west span-100]
@snapend
