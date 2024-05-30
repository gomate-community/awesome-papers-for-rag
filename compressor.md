# Awesome resources about evidence selection component in the RAG system

🔥 **Must-read papers for evidence distillation component in RAG.**

🏃 **Coming soon: Add one-sentence intro to each paper.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

The retrieved documents often contain a list of passages which are ranked by their relevance score to the question. It would be costly to directly input these passages into the LLM. One one hand, the relevance score of these passages does not necessarily indicate their usefulness for answer generation, which could introduce noise to the LLM. On the other hand, the length of the list could exceed the length limit of the LLM. Thus, the evidence distillation (also called compressor) component is introduced to select and compress the retrieved content.



## Table of Content (ToC)


- [Selective Methods](#selection) 
Selective Methods aims to select a subset of tokens from original contexts. 
- [Abstractive Methods](#abstractive) 
Abstractive Methods usually compress contexts by generating summarys.


## 1. Selective Methods <a id="methods"></a>
| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/03/21| [FIT-RAG: Black-Box RAG with Factual Information and Token Reduction](https://arxiv.org/pdf/2403.14374) |Yuren Mao, Xuemei Dong, Wenyi Xu, et al. |Zhejiang University |<small>**FIT-RAG** utilizes the factual information in the retrieval and reduces the number of tokens for augmentation. It consists of five components: a similarity-based retriever, a bi-label document scorer, a bi-faceted self-knowledge recognizer, a sub-document-level token reducer and a prompt construction module.</small>|
|2024/03/19| [LLMLingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) |Zhuoshi Pan, Qianhui Wu, et al. |Microsoft Corporation |<small>**LLMLingua-2** formulate prompt compression as a token classification problem to guarantee the faithfulness of the compressed prompt to the original one, and use a Transformer encoder as the base architecture to capture all essential information for prompt compression from the full bidirectional context.  </small>|
|2023/11/14| [Learning to Filter Context for Retrieval-Augmented Generation](https://arxiv.org/pdf/2311.08377) |Zhiruo Wang, Jun Araki, et al. |Carnegie Mellon University |<small>**FILCO** improves the quality of the context provided to the generator by (1) identifying useful context based on lexical and information-theoretic approaches, and (2) training context filtering models that can filter retrieved contexts at test time.</small>|
|2023/10/10| [LongLLMLingua: Accelerating and Enhancing LLMs in Long Context Scenarios via Prompt Compression](https://arxiv.org/abs/2310.06839) |Huiqiang Jiang, Qianhui Wu, et al. |Microsoft Corporation |<small>**LongLLMLingua** conducts prompt compression towards improving LLMs’ perception of the key information to address three challenges: higher computational/financial cost, longer latency, and inferior performance. </small>|
|2023/10/09| [LLMLingua: Compressing Prompts for Accelerated Inference of Large Language Models](https://arxiv.org/abs/2310.05736) |Huiqiang Jiang, Qianhui Wu, et al. |Microsoft Corporation |<small>**LLMLingua** is a coarse-to-fine prompt compression method that involves a budget controller to maintain semantic integrity under high compression ratios, a token-level iterative compression algorithm to better model the interdependence between compressed contents, and an instruction tuning based method for distribution alignment between language models.  </small>|
|2023/09/02| [LeanContext: Cost-Efficient Domain-Specific Question Answering Using LLMs](https://arxiv.org/abs/2309.00841) |Md Adnan Arefeen, Biplob Debnath, Srimat Chakradhar |NEC Laboratories America |<small>**LeanContext** extracts k key sentences from the context that are closely aligned with the query. LeanContext introduces a reinforcement learning technique that dynamically determines k based on the query and context. The rest of the less important sentences are reduced using a free open source text reduction method. </small>|





## 2. Abstractive Methods <a id="abstractive"></a>


| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/10/25| [TCRA-LLM: Token Compression Retrieval Augmented Large Language Model for Inference Cost Reduction](https://arxiv.org/abs/2310.15556) |Junyi Liu, Liangzhi Li, et al. |Meetyou AI Lab|<small>**TCRA** propose a token compression scheme that includes two methods: summarization compression and semantic compression. The first method applies a T5-based model that is fine-tuned by datasets generated using self-instruct containing samples with varying lengths and reduce token size by doing summarization. The second method further compresses the token size by removing words with lower impact on the semantic.</small>|
|2023/04/12| [RECOMP: Improving Retrieval-Augmented LMs With Compression and Selective Augmentation](https://arxiv.org/pdf/2310.04408.pdf) <br>[[code](https://github.com/carriex/recomp): ![](https://img.shields.io/github/stars/carriex/recomp.svg?style=social)|Fangyuan Xu, Weijia Shi, Eunsol Choi1 |The University of Texas at Austin, University of Washington|<small>**Recomp** introduces two types of compressors: an <u>extractive</u> compressor that selects pertinent sentences from retrieved documents, and an <u>abstractive</u> compressor that produces concise summaries by amalgamating information from multiple documents.</small>|
