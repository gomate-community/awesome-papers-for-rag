# Awesome resources about evidence selection component in the RAG system

🔥 **Must-read papers for evidence distillation component in RAG.**

🏃 **Coming soon: Add one-sentence intro to each paper.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

The retrieved documents often contain a list of passages which are ranked by their relevance score to the question. It would be costly to directly input these passages into the LLM. One one hand, the relevance score of these passages does not necessarily indicate their usefulness for answer generation, which could introduce noise to the LLM. On the other hand, the length of the list could exceed the length limit of the LLM. Thus, the evidence distillation (also called compressor) component is introduced to select and compress the retrieved content.



## Table of Content (ToC)


- [Selective Methods](#selection)
- [Abstractive Methods](#abstractive)


## 1. Selective Methods <a id="methods"></a>
| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/03/21| [FIT-RAG: Black-Box RAG with Factual Information and Token Reduction](https://arxiv.org/pdf/2403.14374) |Yuren Mao, Xuemei Dong, Wenyi Xu, et al. |Zhejiang University |<small>**FIT-RAG** utilizes the factual information in the retrieval and reduces the number of tokens for augmentation. It consists of five components: a similarity-based retriever, a bi-label document scorer, a bi-faceted self-knowledge recognizer, a sub-document-level token reducer and a prompt construction module.</small>|



## 2. Abstractive Methods <a id="abstractive"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/04/12| [RECOMP: Improving Retrieval-Augmented LMs With Compression and Selective Augmentation](https://arxiv.org/pdf/2310.04408.pdf) <br>[[code](https://github.com/carriex/recomp): ![](https://img.shields.io/github/stars/carriex/recomp.svg?style=social)|Fangyuan Xu, Weijia Shi, Eunsol Choi1 |The University of Texas at Austin, University of Washington|<small>**Recomp** introduces two types of compressors: an <u>extractive</u> compressor that selects pertinent sentences from retrieved documents, and an <u>abstractive</u> compressor that produces concise summaries by amalgamating information from multiple documents.</small>|
