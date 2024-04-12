# Awesome resources about rank component in the RAG system

🔥 **Must-read papers for generate component in RAG.**

🏃 **Coming soon: Add one-sentence intro to each paper.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

Coming soon ...


## Table of Content (ToC)


- [Instruction Fine-tuning](#ift)
  - [Outside Module](#otm)
- [Datasets](#datasets)
  - [Factoid QA](#fqa)
  - [Long-form QA](#lfqa)
- [Metrics](#metrics)
  - [Claim Verification](#claimverification)





## 1. Instruction Fine-tuning <a id="ift"></a>

### 1.1 Outside Module <a id="otm"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/5/18| [Augmented Large Language Models with Parametric Knowledge Guiding](https://arxiv.org/abs/2305.04757) | Ziyang Luo, Can Xu, Pu Zhao, et. al.,| Hong Kong Baptist University, Microsoft| <small>This work propose Parametric Knowledge Guiding (**PKG**), which injects domain knowledge for LLaMa-7B via instruction fine-tuning to capture the necessary expertise. Then, the PKG is used to generage context for a given question as the background-augmented prompting for LLMs.</small>|


## 2. Datasets <a id="datasets"></a>

### 2.1 Factoid QA <a id="fqa"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2022/04/12| [ASQA: Factoid Questions Meet Long-Form Answers](https://arxiv.org/abs/2204.06092.pdf)] [[dataset](https://huggingface.co/datasets/din0s/asqa)]|Ivan Stelmakh, Yi Luan, Bhuwan Dhingra, Ming-Wei Chang|Carnegie Mellon University, Duke University, Google Research |<small>ASQA is the first long-form question answering dataset that focuses on ambiguous factoid questions.</small>|
|2024/01/26 | [Benchmarking Large Language Models in Complex Question Answering Attribution using Knowledge Graphs](https://arxiv.org/abs/2401.14640.pdf)| Nan Hu, Jiaoyan Chen, Yike Wu, Guilin Qi, Sheng Bi, Tongtong Wu, Jeff Z. Pan.|Southeast University, The University of Manchester,The University of Edinburgh |<small>CAQA is a new benchmark for complex question answering attribution, which is designed to evaluate the ability of LLMs to answer complex questions with the help of knowledge graphs.</small>|
### 2.1 Long-form QA <a id="lfqa"></a>

## 3. Metrics <a id="metrics"></a>

### 3.1 Claim Verification <a id="claimverification"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/02/23 |[Merging Facts, Crafting Fallacies: Evaluating the Contradictory Nature of Aggregated Factual Claims in Long-Form Generations](https://arxiv.org/abs/2402.05629.pdf)| heng-Han Chiang, Hung-yi Lee.|National Taiwan University|<small>This work finds that combining factual claims together can result in a non-factual paragraph due to entity ambiguity. Current metrics for fact verification fail to properly evaluate these non-factual passages. The authors proposed D-FActScore based on FActScore, and showed the methods and results of human and automatic evaluation.</small>|