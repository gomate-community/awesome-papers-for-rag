# Awesome resources about rank component in the RAG system

🔥 **Must-read papers for rank component in RAG.**

🏃 **Coming soon: Add one-sentence intro to each paper.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

Coming soon ...


## Table of Content (ToC)


- [Retrieval Stage](#retrieval)
  - [Tuning Embeddings](#tunembedding)
  - [Adapting LLM as Retriever](#aligning)
  - [LLM-guided Retriever](#llm-guided-retriever)
  - [Adapter](#adapter)
  - [Data Sources](#datasources)
- [Rerank Stage](#rerank)
  - [Adapting LLM as Reranker](#llm-based-ranker)
  - [Sub-title 2](#2-sub-rerank)






## 1. Retrieval Stage <a id="retrieval"></a>

### 1.1 Tuning Embeddings <a id="tunembedding"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/3/29| [Gecko: Versatile Text Embeddings Distilled from Large Language Models](https://arxiv.org/pdf/2403.20327) | Jinhyuk Lee, Zhuyun Dai, Xiaoqi Ren, et. al.| Google Deepmind|<small>This work present **Gecko**, a compact and versatile text embedding modle, which employs a two-stage distillation process by generating data and refining data quality based on large language models</small>|
|2024/2/23| [Repetition Improves Language Model Embeddings](https://arxiv.org/pdf/2402.15449.pdf) <br>[[code](https://github.com/jakespringer/echo-embeddings): ![](https://img.shields.io/github/stars/jakespringer/echo-embeddings.svg?style=social)] |Jacob Mitchell Springer, Suhas Kotha, Daniel Fried, et. al.| CMU| <small>This work present "**echo embeddings**", in which they repeat the input twice in context and extract embeddings from the second occurrence (i.e., repetition captures bidirectional information)</small>|
|2024/2/15| [Generative Representational Instruction Tuning](https://arxiv.org/abs/2402.09906.pdf), <br>[[code](https://github.com/ContextualAI/gritlm): ![](https://img.shields.io/github/stars/ContextualAI/gritlm.svg?style=social)]|Niklas Muennighoff, Hongjin Su, Liang Wang, et. al. | Contextual AI, The University of Hong Kong, Microsoft|<small>This work introduces generative representational instruction tuning (**GRIT**) whereby a large language model is trained to handle both generative and embedding tasks by distinguishing between them through instructions</small>|
|2024/2/10 | [BGE M3-Embedding: Multi-Lingual, Multi-Functionality,Multi-Granularity Text Embeddings Through Self-Knowledge Distillation](https://arxiv.org/abs/2402.03216.pdf)|Liang Wang, Nan Yang, Xiaolong Huang, et. al.|BAAI, USTC|<small>This work present a new embedding model, called **M3-Embedding**, which is distinguished for its versatility in Multi-Linguality, Multi-Functionality, and Multi-Granularity</small>|
|2024/1/19| [Improving Text Embeddings with Large Language Models](https://arxiv.org/abs/2401.00368.pdf)| Jianlv Chen, Shitao Xiao, Peitian Zhang, et. al.|Microsoft|<small>This work introduce a novel and simple method for obtaining high-quality text embeddings using only synthetic data and less than 1k training steps.</small>|
|2023/10/25|[Retrieve Anything To Augment Large Language Models](https://arxiv.org/abs/2310.07554)]<br>[[code](https://github.com/FlagOpen/FlagEmbedding): ![](https://img.shields.io/github/stars/FlagOpen/FlagEmbedding.svg?style=social)]|AutPeitian Zhang, Shitao Xiao, Zheng Liu, et. al.|BAAI, Renmin Univeristy of China, University of Montreal|<small>This work present a novel approach, the **LLM-Embedder**, which comprehensively supports the diverse retrieval augmentation needs of LLMs with one unified embedding model.</small>|
|2023/5/30| [One Embedder, Any Task: Instruction-Finetuned Text Embeddings](https://arxiv.org/abs/2212.09741)]<br>[[code](https://github.com/xlang-ai/instructor-embedding): ![](https://img.shields.io/github/stars/xlang-ai/instructor-embedding.svg?style=social)]|Hongjin Su, Weijia Shi, Jungo Kasai, et. al.|University of Hong Kong, University of Washingtong, Meta AI, Allen Institute for AI|<small>This work introduce **INSTRUCTOR**, a new method for computing text embeddings given task instructions: every text input is embedded together with instructions explaining the use case (e.g., task and domain descriptions).</small>|
|2022/9/23| [Promptagator: Few-shot Dense Retrieval From 8 Examples](https://arxiv.org/abs/2209.11755)|Zhuyun Dai, Vincent Y. Zhao, Ji Ma, et. al.|Google Research|<small>This work propose Prompt-base Query Generation for Retriever (**Promptagator**), which leverages large language models (LLM) as a few-shot query generator, and creates task-specific retrievers based on the generated data.</small>|
<!--
|2021/4/12| [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401)|Patrick Lewis, Ethan Perez, Aleksandra Piktus, et. al.|Facebook AI, University College London, New York University|<small>This work augment language model pre-training with a latent knowledge retriever, which allows the model to retrieve and attend over documents from a large corpus such as Wikipedia, used during pre-training, fine-tuning and inference.</small>|
|2020/2/1| [REALM: Retrieval-Augmented Language Model Pre-Training](https://arxiv.org/abs/2002.08909)|Kelvin Guu, Kenton Lee, Zora Tung, et. al.|Google Research|<small>This work  jointly finetunes the retriever with a sequence-to-sequence model.</small>|
-->

### 1.2 Adapting LLM as Retriever<a id="aligning"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/12/24|[Making Large Language Models A Better Foundation For Dense Retrieval](https://arxiv.org/pdf/2312.15503.pdf)] <br>[[code](https://github.com/FlagOpen/FlagEmbedding): ![](https://img.shields.io/github/stars/FlagOpen/FlagEmbedding.svg?style=social)| Chaofan Li, Zheng Liu, Shitao Xiao, et. al.|BAAI, BUPT|<small>This work includes **LLaRA** (LLM Adapted for dense RetriAl), which introduce two pretext training tasks EBAE (Embedding-Based Auto-Encoding) and EBAR (Embedding-Based Auto-Regression) to improve LLaMA for dense retrieval.|


<!--
|2023/12/16| [UPRISE: Universal Prompt Retrieval for Improving Zero-Shot Evaluation](https://arxiv.org/abs/2303.08518.pdf)]<br>[[code](https://github.com/microsoft/LMOps): ![](https://img.shields.io/github/stars/microsoft/LMOps.svg?style=social) |Daixuan Cheng, Shaohan Huang, Junyu Bi, et. al.|Microsoft|<small>This work propose  UPRISE (Universal Prompt Retrieval for Improving zero-Shot Evaluation), which tunes a lightweight and versatile retriever that automatically retrieves prompts for a given zero-shot task input.</small>|
-->

### 1.3 LLM-guided Retriever<a id="llm-guided-retriever"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/5/26| [Augmentation-Adapted Retriever Improves Generalization of Language Models as Generic Plug-In](https://arxiv.org/abs/2305.17331.pdf) <br> [[code](https://github.com/OpenMatch/Augmentation-Adapted-Retriever): ![](https://img.shields.io/github/stars/OpenMatch/Augmentation-Adapted-Retriever.svg?style=social)] |Zichun Yu, Chenyan Xiong, Shi Yu, Zhiyuan Liu|<small>Tsinghua University, Microsoft|<small>This work introduce augmentation-adapted retriever (AAR), which takes a black-box LLM to score positive documents (so called LLM-preferred signals) for fine-tuning a pre-trained retriever.</small>|
|2023/5/24| [REPLUG: Retrieval-Augmented Black-Box Language Models](https://arxiv.org/abs/2301.12652.pdf) |Weijia Shi, Sewon Min, Michihiro Yasunaga, et. al.|University of Washington, Stanford University, KAIST, Meta AI|<small>This work introduce REPLUG, which prepends each retrieved document and question separately to the LLM and ensembles output probabilities from different passes. Besides, it takes LM to score documents to supervise the dense retriever training.</small>|
|2022/11/16| [Atlas: Few-shot Learning with Retrieval Augmented Language Models](https://arxiv.org/abs/2208.03299.pdf)] [[code](https://github.com/facebookresearch/atlas): ![](https://img.shields.io/github/stars/facebookresearch/atlas.svg?style=social)]|Gautier Izacard, Patrick Lewis, Maria Lomeli, et. al.|Meta AI, ENS, PSL University, Inria, UCL|<small>This work present Atlas, a retrieval (Contriever) augmented language model (T5) by carefully designed training, i.e., 1) jointly pre-train the retriever and LLM using unsupervised output, 2) efficient retriever fine-tuning (including full index update, reranking, and query-side fine-tuning).</small>|


### 1.4 Adpter <a id="adapter"></a>


- [2023/5/18] **Augmented Large Language Models with Parametric Knowledge Guiding** *Ziyang Luo, Can Xu, Pu Zhao, Xiubo Geng, Chongyang Tao, Jing Ma, Qingwei Lin, Daxin Jiang* [[paper](https://arxiv.org/abs/2305.04757)] 
  - This work propose the novel Parametric Knowledge Guiding (PKG) framework, which equips LLMs with a knowledge-guiding module to access relevant knowledge without altering the LLMs' parameters.
- [2023/6/22] **Interleaving Retrieval with Chain-of-Thought Reasoning for Knowledge-Intensive Multi-Step Questions** *Harsh Trivedi, Niranjan Balasubramanian, Tushar Khot, Ashish Sabharwal* [[paper](https://arxiv.org/abs/2212.10509)] [[code](https://github.com/stonybrooknlp/ircot), ![](https://img.shields.io/github/stars/stonybrooknlp/ircot.svg?style=social)]
  - This work propose IRCoT, a new approach for multi-step QA that interleaves retrieval with steps (sentences) in a CoT, guiding the retrieval with CoT and in turn using retrieved results to improve CoT.
- [2023/10/8] **Retrieval-Generation Synergy Augmented Large Language Models** *Zhangyin Feng, Xiaocheng Feng, Dezhi Zhao, Maojin Yang, Bing Qin* [[paper](https://arxiv.org/abs/2310.05149)] 
  - This work present ITRG, which is an iterative retrieval-generation synergy framework, containing two important steps: generation-augmented retrieval and retrieval-augmented generation. They form a closed loop, and can improve each other via multiple iterations.

### 1.5 Data Sources <a id="datasources"></a>

- [2023/10/8] **Self-Knowledge Guided Retrieval Augmentation for Large Language Models** *Yile Wang, Peng Li, Maosong Sun, Yang Liu* [[paper](https://arxiv.org/abs/2310.05002)] 
  - This work nvestigate eliciting the model's ability to recognize what they know and do not know (which is also called self-knowledge) and propose Self-Knowledge guided Retrieval augmentation (SKR), a simple yet effective method which can let LLMs refer to the questions they have previously encountered and adaptively call for external resources when dealing with new questions.



## 2. Rerank Stage <a id="rerank"></a>

### 2.1 Adapting LLM as Reranker <a id="llm-based-ranker"></a>
| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/12/5 | [Rank-without-GPT: Building GPT-Independent Listwise Rerankers on Open-Source Large Language Models](https://arxiv.org/pdf/2312.02969.pdf)] [[code](https://huggingface.co/castorini)] | Xinyu Zhang, Sebastian Hofstätter, Patrick Lewis, et al.|University of Waterloo, Cohere, Comcast Applied AI|<small>This work finetunes LLaMA model both as a dense retriever (RepLLaMA) and as a point-wise reranker (RankLLaMA) for both passage retrieval and document retrieval using the MS MARCO datasets.</small>|
|2023/10/12 | [Fine-Tuning LLaMA for Multi-Stage Text Retrieval](https://arxiv.org/pdf/2310.08319.pdf)| Xueguang Ma, Liang Wang, Nan Yang et al.|David R. Cheriton School of Computer Science, University of Waterloo, Microsoft Research|<small>This work studies how to construct GPT-free listwise rerankers based on open-source LLM models</small>|
|2023/5/1| [Say Goodbye to Irrelevant Search Results: Cohere Rerank Is Here](https://txt.cohere.com/rerank)| NILS REIMERS, SYLVIE SHI, LUCAS FAYOUX, ELLIOTT CHOI| Cohere| <small>This work propose Cohere Rerank,which can provide a powerful semantic boost to the search quality of any keyword or vector search system without requiring any overhaul or replacement.</small>|
