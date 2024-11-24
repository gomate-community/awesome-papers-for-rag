# Awesome resources about generator component in the RAG system

🔥 **Must-read papers for generator component in RAG.**

🏃 **Coming soon: Add one-sentence intro to each paper.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

Coming soon ...


## Table of Content (ToC)


- [Instruction Fine-tuning](#ift)
  - [Outside Module](#otm)
- [Attribution Augmentation](#attribution)
  - [Post-process Method](#post)
- [Hallucinations](#hallucination)
- [Datasets](#datasets)
  - [Factoid QA](#fqa)
  - [Long-form QA](#lfqa)





## 1. Instruction Fine-tuning <a id="ift"></a>

### 1.1 Outside Module <a id="otm"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/5/18| [Augmented Large Language Models with Parametric Knowledge Guiding](https://arxiv.org/abs/2305.04757) | Ziyang Luo, Can Xu, Pu Zhao, et. al.,| Hong Kong Baptist University, Microsoft| <details><summary><small>This paper presents PKG ...</small></summary><small>This work propose Parametric Knowledge Guiding (**PKG**), which injects domain knowledge for LLaMa-7B via instruction fine-tuning to capture the necessary expertise. Then, the PKG is used to generage context for a given question as the background-augmented prompting for LLMs.</small></details>|


## 2. Attribution Augmentation <a id="attribution"></a>

### 2.1 Post-Process Method <a id="post"></a>
| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/03/04 | [Citation-Enhanced Generation for LLM-based Chatbots](https://arxiv.org/pdf/2402.16063) | Weitao Li, Junkai Li, Weizhi Ma, Yang Liu | Zhejiang Lab | <details><summary><small>This paper presents CEG ...</small></summary><small>This work proposes a post-hoc Citation-Enhanced Generation (CEG) approach combined with RAG. It consists of three components: 1) *Retrieval Augmentation Module* uses NLTK as sentence tokenizer to obtain claims, then uses dense retrieval (SimCSE Bert) to retrieve documents; 2) *Citation Generation Module* first uses NLI model to determine the relationship between each claim-document pair to select valid reference for each claim; 3) *Response Regeneration Module* takes the question, original response, nonfactual claims, and relevant docs, as prompt input to regenerate the new response.</small></details>|

## 3. Haullucinations <a id="hallucinations"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/09/13 | [Cognitive Mirage: A Review of Hallucinations in Large Language Models](https://arxiv.org/pdf/2309.06794.pdf) | Hongbin Ye, Tong Liu, Aijia Zhang, Wei Hua, Weiqiang Jia | Zhejiang Lab | <details><summary><small>This paper presents taxonomy of hallucinations ...</small></summary><small>This work provides a literature review on hallucinations, which presents a taxonomy of hallucinations from several text generation tasks, and mechanism analysis (three types: data collection, knowledge gap, and optimization process), detection methods and improvement approaches.</small></details>|

## 4. Datasets <a id="datasets"></a>

### 4.1 Factoid QA <a id="fqa"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/01/26 | [Benchmarking Large Language Models in Complex Question Answering Attribution using Knowledge Graphs](https://arxiv.org/abs/2401.14640.pdf)| Nan Hu, Jiaoyan Chen, Yike Wu, Guilin Qi, Sheng Bi, Tongtong Wu, Jeff Z. Pan.|Southeast University, The University of Manchester,The University of Edinburgh |<details><summary><small>This paper presents CAQA ...</small></summary><small>CAQA is a new benchmark for complex question answering attribution, which is designed to evaluate the ability of LLMs to answer complex questions with the help of knowledge graphs.</small></details>|
|2022/04/12| [ASQA: Factoid Questions Meet Long-Form Answers](https://arxiv.org/abs/2204.06092.pdf) [[dataset](https://huggingface.co/datasets/din0s/asqa)]|Ivan Stelmakh, Yi Luan, Bhuwan Dhingra, Ming-Wei Chang|Carnegie Mellon University, Duke University, Google Research |<details><summary><small>This paper presents ASQA ...</small></summary><small>ASQA is the first long-form question answering dataset that focuses on ambiguous factoid questions.</small></details>|

### 4.2 Long-form QA <a id="lfqa"></a>

