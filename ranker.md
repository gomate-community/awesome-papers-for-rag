# Awesome resources about rank component in the RAG system

🔥 **Must-read papers for rank component in RAG.**

🏃 **Coming soon: Add one-sentence intro to each paper.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

Coming soon ...


## Table of Content (ToC)


- [Retrieval Stage](#retrieval)
  - [Fine-tuning Embedding Models](#tunembedding)
  - [Aligning Retriever and LLM](#aligning)
  - [Adapter](#adapter)
  - [Data Sources](#datasources)
- [Rerank Stage](#rerank)
  - [Sub-title 1](#1-sub-rerank)
  - [Sub-title 2](#2-sub-rerank)






## 1. Retrieval Stage <a id="retrieval"></>

### 1.1 Fine-tuning Embedding Models <a id="tunembedding"></>




- [2024/2/10] **BGE M3-Embedding: Multi-Lingual, Multi-Functionality,Multi-Granularity Text Embeddings Through Self-Knowledge Distillation** *Liang Wang, Nan Yang, Xiaolong Huang, et. al.* [[paper](https://arxiv.org/abs/2401.00368)] 
  - This work present a new embedding model, called M3-Embedding, which is distinguished for its versatility in Multi-Linguality, Multi-Functionality, and Multi-Granularity.
- [2024/1/19] **Improving Text Embeddings with Large Language Models** *Jianlv Chen, Shitao Xiao, Peitian Zhang, et. al.* [[paper](https://arxiv.org/abs/2402.03216)]
  - This work introduce a novel and simple method for obtaining high-quality text embeddings using only synthetic data and less than 1k training steps.
- [2023/10/25] **Retrieve Anything To Augment Large Language Models** *AutPeitian Zhang, Shitao Xiao, Zheng Liu, et. al. * [[paper](https://arxiv.org/abs/2310.07554)] [[code](https://github.com/FlagOpen/FlagEmbedding), ![](https://img.shields.io/github/stars/FlagOpen/FlagEmbedding.svg?style=social)]
  - This work present a novel approach, the LLM-Embedder, which comprehensively supports the diverse retrieval augmentation needs of LLMs with one unified embedding model.
- [2023/5/30] **One Embedder, Any Task: Instruction-Finetuned Text Embeddings** *Hongjin Su, Weijia Shi, Jungo Kasai, et. al. * [[paper](https://arxiv.org/abs/2212.09741)] [[code](https://github.com/xlang-ai/instructor-embedding), ![](https://img.shields.io/github/stars/xlang-ai/instructor-embedding.svg?style=social)]
  - This work introduce INSTRUCTOR, a new method for computing text embeddings given task instructions: every text input is embedded together with instructions explaining the use case (e.g., task and domain descriptions).
- [2022/9/23] **Promptagator: Few-shot Dense Retrieval From 8 Examples** *Zhuyun Dai, Vincent Y. Zhao, Ji Ma, et. al. * [[paper](https://arxiv.org/abs/2209.11755)]
  - This work propose Prompt-base Query Generation for Retriever (Promptagator), which leverages large language models (LLM) as a few-shot query generator, and creates task-specific retrievers based on the generated data.
- [2021/4/12] **Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks** *Patrick Lewis, Ethan Perez, Aleksandra Piktus, et. al.* [[paper](https://arxiv.org/abs/2005.11401)] 
  - This work augment language model pre-training with a latent knowledge retriever, which allows the model to retrieve and attend over documents from a large corpus such as Wikipedia, used during pre-training, fine-tuning and inference.
- [2020/2/1] **REALM: Retrieval-Augmented Language Model Pre-Training** *Kelvin Guu, Kenton Lee, Zora Tung, et. al.* [[paper](https://arxiv.org/abs/2002.08909)] 
  - This work  jointly finetunes the retriever with a sequence-to-sequence model.

### 1.2 Aligning Retriever and LLM <a id="aligning"></>


- [2023/12/16] **UPRISE: Universal Prompt Retrieval for Improving Zero-Shot Evaluation** *Daixuan Cheng, Shaohan Huang, Junyu Bi, et. al.* [[paper](https://arxiv.org/abs/2303.08518)] [[code](https://github.com/microsoft/LMOps), ![](https://img.shields.io/github/stars/microsoft/LMOps.svg?style=social)]
  - This work propose  UPRISE (Universal Prompt Retrieval for Improving zero-Shot Evaluation), which tunes a lightweight and versatile retriever that automatically retrieves prompts for a given zero-shot task input.
- [2023/5/26] **Augmentation-Adapted Retriever Improves Generalization of Language Models as Generic Plug-In** *Zichun Yu, Chenyan Xiong, Shi Yu, Zhiyuan Liu* [[paper](https://arxiv.org/abs/2305.17331)] [[code](https://github.com/OpenMatch/Augmentation-Adapted-Retriever), ![](https://img.shields.io/github/stars/OpenMatch/Augmentation-Adapted-Retriever.svg?style=social)]
  - This work propose augmentation-adapted retriever (AAR), which learns LM's preferences obtained from a known source LM to retrieve useful documents for unseen target LMs.
- [2023/5/24] **REPLUG: Retrieval-Augmented Black-Box Language Models** *Weijia Shi, Sewon Min, Michihiro Yasunaga, et. al.* [[paper](https://arxiv.org/abs/2301.12652)] 
  - This work introduce REPLUG, a retrieval-augmented language modeling framework that treats the language model (LM) as a black box and augments it with a tuneable retrieval model and show that the LM can be used to supervise the retrieval model, which can then find documents that help the LM make better predictions.
- [2022/11/16] **Atlas: Few-shot Learning with Retrieval Augmented Language Models** *Gautier Izacard, Patrick Lewis, Maria Lomeli, et. al.* [[paper](https://arxiv.org/abs/2208.03299)] [[code](https://github.com/facebookresearch/atlas), ![](https://img.shields.io/github/stars/facebookresearch/atlas.svg?style=social)]
  - This work present Atlas, a carefully designed and pre-trained retrieval augmented language model able to learn knowledge intensive tasks with very few training examples.

### 1.3 Adpter <a id="adapter"></>

- [2022/12/31] **Rethinking with Retrieval: Faithful Large Language Model Inference** *Hangfeng He, Hongming Zhang, Dan Roth* [[paper](https://arxiv.org/abs/2301.00303)] [[code](https://github.com/HornHehhf/RR), ![](https://img.shields.io/github/stars/HornHehhf/RR.svg?style=social)]
  - This work propose a novel post-processing approach, rethinking with retrieval (RR), which retrieves relevant external knowledge based on the decomposed reasoning steps obtained from the chain-of-thought (CoT) prompting.
- [2023/5/18] **Augmented Large Language Models with Parametric Knowledge Guiding** *Ziyang Luo, Can Xu, Pu Zhao, Xiubo Geng, Chongyang Tao, Jing Ma, Qingwei Lin, Daxin Jiang* [[paper](https://arxiv.org/abs/2305.04757)] 
  - This work propose the novel Parametric Knowledge Guiding (PKG) framework, which equips LLMs with a knowledge-guiding module to access relevant knowledge without altering the LLMs' parameters.
- [2023/6/22] **Interleaving Retrieval with Chain-of-Thought Reasoning for Knowledge-Intensive Multi-Step Questions** *Harsh Trivedi, Niranjan Balasubramanian, Tushar Khot, Ashish Sabharwal* [[paper](https://arxiv.org/abs/2212.10509)] [[code](https://github.com/stonybrooknlp/ircot), ![](https://img.shields.io/github/stars/stonybrooknlp/ircot.svg?style=social)]
  - This work propose IRCoT, a new approach for multi-step QA that interleaves retrieval with steps (sentences) in a CoT, guiding the retrieval with CoT and in turn using retrieved results to improve CoT.
- [2023/10/8] **Retrieval-Generation Synergy Augmented Large Language Models** *Zhangyin Feng, Xiaocheng Feng, Dezhi Zhao, Maojin Yang, Bing Qin* [[paper](https://arxiv.org/abs/2310.05149)] 
  - This work present ITRG, which is an iterative retrieval-generation synergy framework, containing two important steps: generation-augmented retrieval and retrieval-augmented generation. They form a closed loop, and can improve each other via multiple iterations.

### 1.4 Data Sources <a id="datasources"></a>

- [2023/10/8] **Self-Knowledge Guided Retrieval Augmentation for Large Language Models** *Yile Wang, Peng Li, Maosong Sun, Yang Liu* [[paper](https://arxiv.org/abs/2310.05002)] 
  - This work nvestigate eliciting the model's ability to recognize what they know and do not know (which is also called self-knowledge) and propose Self-Knowledge guided Retrieval augmentation (SKR), a simple yet effective method which can let LLMs refer to the questions they have previously encountered and adaptively call for external resources when dealing with new questions.



## 2. Rerank Stage <a id="rerank"></a>

### 2.1 Sub-title 1

- [2023/5/1] **Say Goodbye to Irrelevant Search Results: Cohere Rerank Is Here** *NILS REIMERS, SYLVIE SHI, LUCAS FAYOUX, ELLIOTT CHOI* [[paper](https://txt.cohere.com/rerank)] 
  - This work propose Cohere Rerank,which can provide a powerful semantic boost to the search quality of any keyword or vector search system without requiring any overhaul or replacement.
