# Awesome resources about compressor component in the RAG system

🔥 **Must-read papers for compressor component in RAG.**

🏃 **Coming soon: Add one-sentence intro to each paper.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

The retrieved documents often contain a list of passages which are ranked by their relevance score to the question. It would be costly to directly input these passages into the LLM. One one hand, the relevance score of these passages does not necessarily indicate their usefulness for answer generation, which could introduce noise to the LLM. On the other hand, the length of the list could exceed the length limit of the LLM. Thus, the compressor component is introduced to select and compress the retrieved content.



## Table of Content (ToC)


- [Evidence Selection Method](#selection)
- [Content Compression Method](#compression)


## 1. Evidence Selection Method <a id="methods"></a>



## 2. Content Compression Method <a id="datasets"></a>

- [2022/04/12] **RECOMP: Improving Retrieval-Augmented LMs With Compression and Selective Augmentation** *Fangyuan Xu, Weijia Shi, Eunsol Choi1* [[paper](https://arxiv.org/pdf/2310.04408.pdf)] [[code](https://github.com/carriex/recomp), ![](https://img.shields.io/github/stars/carriex/recomp.svg?style=social)]
  - **Recomp** introduces two types of compressors: an extractive compressor that selects pertinent sentences from retrieved documents, and an abstractive compressor that produces concise summaries by amalgamating information from multiple documents.
