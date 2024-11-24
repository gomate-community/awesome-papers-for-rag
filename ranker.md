# Awesome resources about retrieval component in the RAG system

🔥 **Must-read papers for retrieval component in RAG.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

Coming soon ...


## Table of Content (ToC)


- [Retrieval Methods](#retrieval)
  - [Two-tower Retriever (Tuning Embeddings)](#tunembedding)
  - [Adapting LLM as Retriever](#aligning)
  - [LLM-guided Retriever](#llm-guided-retriever)
  - [Structured Retriever](#structured-retriever)

- [Analysis about Retrieval](#analysis)





## 1. Retrieval Methods <a id="retrieval"></a>

### 1.1 Two-tower Retriever (Tuning Embeddings) <a id="tunembedding"></a>

| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/3/29| [Gecko: Versatile Text Embeddings Distilled from Large Language Models](https://arxiv.org/pdf/2403.20327) | Jinhyuk Lee, Zhuyun Dai, Xiaoqi Ren, et. al.| Google Deepmind|<details><summary><small>This paper presents Gecko ...</small></summary><small>This work present **Gecko**, a compact and versatile text embedding modle, which employs a two-stage distillation process by generating data and refining data quality based on large language models</small></details>| <sub>MTEB</sub>|
|2024/2/23| [Repetition Improves Language Model Embeddings](https://arxiv.org/pdf/2402.15449.pdf) <br>[[code](https://github.com/jakespringer/echo-embeddings): ![](https://img.shields.io/github/stars/jakespringer/echo-embeddings.svg?style=social)] |Jacob Mitchell Springer, Suhas Kotha, Daniel Fried, et. al.| CMU| <details><summary><small>This paper presents echo embeddings ...</small></summary><small>This work present "**echo embeddings**", in which they repeat the input twice in context and extract embeddings from the second occurrence (i.e., repetition captures bidirectional information)</small></details>| <sub>MTEB</sub>|
|2024/2/15| [Generative Representational Instruction Tuning](https://arxiv.org/abs/2402.09906.pdf), <br>[[code](https://github.com/ContextualAI/gritlm): ![](https://img.shields.io/github/stars/ContextualAI/gritlm.svg?style=social)]|Niklas Muennighoff, Hongjin Su, Liang Wang, et. al. | Contextual AI, The University of Hong Kong, Microsoft|<details><summary><small>This paper presents GRIT ...</small></summary><small>This work introduces generative representational instruction tuning (**GRIT**) whereby a large language model is trained to handle both generative and embedding tasks by distinguishing between them through instructions</small></details>| <sub>MTEB</sub>|
|2024/2/10 | [BGE M3-Embedding: Multi-Lingual, Multi-Functionality,Multi-Granularity Text Embeddings Through Self-Knowledge Distillation](https://arxiv.org/abs/2402.03216.pdf)|Liang Wang, Nan Yang, Xiaolong Huang, et. al.|BAAI, USTC|<details><summary><small>This paper presents M3-embedding ...</small></summary><small>This work present a new embedding model, called **M3-Embedding**, which is distinguished for its versatility in Multi-Linguality, Multi-Functionality, and Multi-Granularity</small></details>| <sub>MIRACL, MKQA, MLDR</sub>|
|2024/1/19| [Improving Text Embeddings with Large Language Models](https://arxiv.org/abs/2401.00368.pdf)| Jianlv Chen, Shitao Xiao, Peitian Zhang, et. al.|Microsoft|<details><summary><small>This paper presents ...</small></summary><small>This work introduce a novel and simple method for obtaining high-quality text embeddings using only synthetic data and less than 1k training steps.</small></details>| <sub> BEIR, MTEB</sub>|
|2023/10/25|[Retrieve Anything To Augment Large Language Models](https://arxiv.org/abs/2310.07554)<br>[[code](https://github.com/FlagOpen/FlagEmbedding): ![](https://img.shields.io/github/stars/FlagOpen/FlagEmbedding.svg?style=social)]|AutPeitian Zhang, Shitao Xiao, Zheng Liu, et. al.|BAAI, Renmin Univeristy of China, University of Montreal|<details><summary><small>This paper presents LLM-Embedder ...</small></summary><small>This work present a novel approach, the **LLM-Embedder**, which comprehensively supports the diverse retrieval augmentation needs of LLMs with one unified embedding model.</small></details>| <sub>MMLU, PopQA</sub>|
|2023/5/30| [One Embedder, Any Task: Instruction-Finetuned Text Embeddings](https://arxiv.org/abs/2212.09741)<br>[[code](https://github.com/xlang-ai/instructor-embedding): ![](https://img.shields.io/github/stars/xlang-ai/instructor-embedding.svg?style=social)]|Hongjin Su, Weijia Shi, Jungo Kasai, et. al.|University of Hong Kong, University of Washingtong, Meta AI, Allen Institute for AI|<details><summary><small>This paper presents INSTRUCTOR ...</small></summary><small>This work introduce **INSTRUCTOR**, a new method for computing text embeddings given task instructions: every text input is embedded together with instructions explaining the use case (e.g., task and domain descriptions).</small></details>| <sub>MTEB</sub>|
|2022/9/23| [Promptagator: Few-shot Dense Retrieval From 8 Examples](https://arxiv.org/abs/2209.11755)|Zhuyun Dai, Vincent Y. Zhao, Ji Ma, et. al.|Google Research|<details><summary><small>This paper presents Promptagator ...</small></summary><small>This work propose Prompt-base Query Generation for Retriever (**Promptagator**), which leverages large language models (LLM) as a few-shot query generator, and creates task-specific retrievers based on the generated data.</small></details>| <sub>BEIR</sub>|
<!--
|2021/4/12| [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401)|Patrick Lewis, Ethan Perez, Aleksandra Piktus, et. al.|Facebook AI, University College London, New York University|<details><summary><small>This paper presents ...</small></summary><small>This work augment language model pre-training with a latent knowledge retriever, which allows the model to retrieve and attend over documents from a large corpus such as Wikipedia, used during pre-training, fine-tuning and inference.</small></details>| <sub></sub>|
|2020/2/1| [REALM: Retrieval-Augmented Language Model Pre-Training](https://arxiv.org/abs/2002.08909)|Kelvin Guu, Kenton Lee, Zora Tung, et. al.|Google Research|<details><summary><small>This paper presents REALM ...</small></summary><small>This work jointly finetunes the retriever with a sequence-to-sequence model.</small></details>| <sub></sub>|
-->

### 1.2 Adapting LLM as Retriever<a id="aligning"></a>

| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/12/24|[Making Large Language Models A Better Foundation For Dense Retrieval](https://arxiv.org/pdf/2312.15503.pdf) <br>[[code](https://github.com/FlagOpen/FlagEmbedding): ![](https://img.shields.io/github/stars/FlagOpen/FlagEmbedding.svg?style=social)]| Chaofan Li, Zheng Liu, Shitao Xiao, et. al.|BAAI, BUPT|<details><summary><small>This paper presents LLaRA ...</small></summary><small>This work includes **LLaRA** (LLM Adapted for dense RetriAl), which introduce two pretext training tasks EBAE (Embedding-Based Auto-Encoding) and EBAR (Embedding-Based Auto-Regression) to improve LLaMA for dense retrieval.</small></details>|<sub>MS MARCO passage&document, BEIR</sub>|


<!--
|2023/12/16| [UPRISE: Universal Prompt Retrieval for Improving Zero-Shot Evaluation](https://arxiv.org/abs/2303.08518.pdf)<br>[[code](https://github.com/microsoft/LMOps): ![](https://img.shields.io/github/stars/microsoft/LMOps.svg?style=social) |Daixuan Cheng, Shaohan Huang, Junyu Bi, et. al.|Microsoft|<details><summary><small>This paper presents UPRISE ...</small></summary><small>This work propose  UPRISE (Universal Prompt Retrieval for Improving zero-Shot Evaluation), which tunes a lightweight and versatile retriever that automatically retrieves prompts for a given zero-shot task input.</small></details>|
-->

### 1.3 LLM-guided Retriever<a id="llm-guided-retriever"></a>

| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/03/27| [LLatrieval: LLM-Verified Retrieval for Verifiable Generation](https://arxiv.org/pdf/2311.07838.pdf)<br>[[code](https://github.com/BeastyZ/LLM-Verified-Retrieval): ![](https://img.shields.io/github/stars/BeastyZ/LLM-Verified-Retrieval.svg?style=social))]| Xiaonan Li, Changtai Zhu, Linyang Li, et. al.| Fudan University | <details><summary><small>This paper presents LLatrieval ...</small></summary><small>This work proposes **LLatrieval** (LLM-verified Retrieval), where the LLM iteratively provides feedback to the retrieval through verify-update iterations. 1) **Retrieval Verification** is implemented by prompting LLM to give binary label, and 2) **Retrieval Update** takes LLM to progressively scan the document candidates returned by the retriever and selects the supporting documents.</small></details>|<sub>ALCE</sub>|
|2024/3/15 | [DRAGIN: Dynamic Retrieval Augmented Generation based on the Real-time Information Needs of Large Language Models](https://arxiv.org/abs/2403.10081) <br>[[code](https://github.com/oneal2000/DRAGIN): ![](https://img.shields.io/github/stars/oneal2000/DRAGIN.svg?style=social)] | Weihang Su, Yichen Tang, Qingyao Ai, Zhijing Wu, Yiqun Liu|  Tsinghua University, Beijing Institute of Technology| <details><summary><small>This paper presents DRAGIN ...</small></summary><small>This work introduce a new framework, **DRAGIN**, i.e., Dynamic Retrieval Augmented Generation based on the real-time Information Needs of LLMs. This framework is specifically designed to make decisions on when and what to retrieve based on the LLM’s real-time information needs during the text generation process.</small></details>|<sub>2WikiMHQA, HotpotQA, IIRC, StrategyQA</sub>|
|2023/5/26| [Augmentation-Adapted Retriever Improves Generalization of Language Models as Generic Plug-In](https://arxiv.org/abs/2305.17331.pdf) <br> [[code](https://github.com/OpenMatch/Augmentation-Adapted-Retriever): ![](https://img.shields.io/github/stars/OpenMatch/Augmentation-Adapted-Retriever.svg?style=social)] |Zichun Yu, Chenyan Xiong, Shi Yu, Zhiyuan Liu|Tsinghua University, Microsoft|<details><summary><small>This paper presents AAR ...</small></summary><small>This work introduce augmentation-adapted retriever (AAR), which takes a black-box LLM to score positive documents (so called LLM-preferred signals) for fine-tuning a pre-trained retriever.</small></details>|<sub>MMLU, PopQA</sub>|


### 1.4 Structured Retriever <a id="structured-retriever"></a>
| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/01/31|[RAPTOR: Recursive Abstractive Processing for Tree-Organized Retrieval](https://arxiv.org/abs/2401.18059) [[code](https://github.com/parthsarthi03/raptor): ![](https://img.shields.io/github/stars/parthsarthi03/raptor.svg?style=social)]|Parth Sarthi, Salman Abdullah, Aditi Tuli, Shubh Khanna, Anna Goldie, Christopher D. Manning|Stanford|<details><summary><small>This paper presents RAPTOR ...</small></summary><small>We introduce the novel approach of recursively embedding, clustering, and summarizing chunks of text, constructing a tree with differing levels of summarization from the bottom up. At inference time, our RAPTOR model retrieves from this tree, integrating information across lengthy documents at different levels of abstraction.  On question-answering tasks that involve complex, multi-step reasoning, we show state-of-the-art results; for example, by coupling RAPTOR retrieval with the use of GPT-4, we can improve the best performance on the QuALITY benchmark by 20% in absolute accuracy.</small></details>|<sub>NarrativeQA, QASPER, QuALITY</sub>|


## 2. Analysis about Retrieval<a id="analysis"></a>

| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/7/14 | [The Power of Noise: Redefining Retrieval for RAG Systems](https://arxiv.org/abs/2401.14887) <br>[[code](https://github.com/florin-git/The-Power-of-Noise): ![](https://img.shields.io/github/stars/florin-git/The-Power-of-Noise.svg?style=social)] | F. Cuconasu, G. Trappolini, F. Siciliano, etl. al.|  Sapienza University of Rome| <details><summary><small>This paper studies noise passages ...</small></summary><small>This paper studied the impact of noise passages in RAG, and found that adding random documents in the prompt improves the LLM accuracy by up to 35% on the NQ dataset.</small></details>|<sub>NQ-open (subset of NQ)</sub>|

