# Awesome resources about generation component in the RAG system

🔥 **Must-read papers for generation component in RAG.**

<!----- 🏃 **Coming soon: Add one-sentence intro to each paper.** -----> 

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

Coming soon ...


## Table of Content (ToC)


- [Generation Ability Enhance](#ift)
  - [Knowledge Enhance](#otm)
  - [Attribution Enhance](#attribution)
  - [Long-context Enhance](#attribution)
- [Hallucinations](#hallucination)
- [Datasets](#datasets)
  - [Factoid QA](#fqa)
  - [Long-form QA](#lfqa)





## 1. Instruction Fine-tuning <a id="ift"></a>

### 1.1 Knowledge Enhance <a id="otm"></a>

| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/03/15 | [RAFT: Adapting Language Model to Domain Specific RAG](https://arxiv.org/abs/2403.10131) [[code](https://github.com/ShishirPatil/gorilla): ![](https://img.shields.io/github/stars/ShishirPatil/gorilla.svg?style=social)]| Tianjun Zhang, Shishir G. Patil, Naman Jain, Sheng Shen, et al.|UC Berkeley|<details><summary><small>This paper presents *RAFT* ...</small></summary><small> RAFT leverages fine-tuning with question-answer pairs while referencing the documents in a simulated imperfect retrieval setting — thereby effectively preparing for the open-book exam setting. The RAFT is trained to answer the question (Q) from Document(s) (D) to generate answer (A), where A includes chain-of-thought reasoning.</small></details>| <sub>PubMed, HotpotQA, Gorilla</sub> |
|2023/5/18| [Augmented Large Language Models with Parametric Knowledge Guiding](https://arxiv.org/abs/2305.04757) | Ziyang Luo, Can Xu, Pu Zhao, et. al.,| Hong Kong Baptist University, Microsoft| <details><summary><small>This paper presents PKG ...</small></summary><small>This work propose Parametric Knowledge Guiding (**PKG**), which injects domain knowledge for LLaMa-7B via instruction fine-tuning to capture the necessary expertise. Then, the PKG is used to generage context for a given question as the background-augmented prompting for LLMs.</small></details>| <sub>FM2, NQ-Table, MedMC-QA, ScienceQA</sub>|


### 1.2 Attribution Enhance <a id="attribution"></a>
| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/08/20 | [INSTRUCTRAG: Instructing Retrieval-Augmented Generation via Self-Synthesized Rationales](https://arxiv.org/pdf/2406.13629) [[code](https://github.com/weizhepei/InstructRAG): ![](https://img.shields.io/github/stars/weizhepei/InstructRAG.svg?style=social)] | Zhepei Wei, Wei-Lin Chen, Yu Meng | University of Virginia | <details><summary><small>This paper presents InstructRAG ...</small></summary><small>This work proposes InstructRAG to generate rationales along with the answer, enhancing both the generation accuracy and trustworthiness. It first prompt an instruction-tuned LLM (rational generator) to synthesize rationales, which is to explain how to derive correct answer from noisy retrieved documents. Then, it guid the LM to learn explict denoising by leveraging these rationals as either in-context learning demonstrations or as supervised fine-tuning data.</small></details>|<sub>PopQA, TriviaQA, NQ, ASQA, 2WikiMHQA </sub>|
|2024/03/04 | [Citation-Enhanced Generation for LLM-based Chatbots](https://arxiv.org/pdf/2402.16063) | Weitao Li, Junkai Li, Weizhi Ma, Yang Liu | Tsinghua University | <details><summary><small>This paper presents CEG ...</small></summary><small>This work proposes a post-hoc Citation-Enhanced Generation (CEG) approach combined with RAG. It consists of three components: 1) *Retrieval Augmentation Module* uses NLTK as sentence tokenizer to obtain claims, then uses dense retrieval (SimCSE Bert) to retrieve documents; 2) *Citation Generation Module* first uses NLI model to determine the relationship between each claim-document pair to select valid reference for each claim; 3) *Response Regeneration Module* takes the question, original response, nonfactual claims, and relevant docs, as prompt input to regenerate the new response.</small></details>|<sub>WikiBio GPT-3, FELM, HaluEval, WikiRetr </sub>|

### 1.3 Long-context Enhance <a id="attribution"></a>
| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/07/11 | [LLM Maybe LongLM: SelfExtend LLM Context Window Without Tuning](https://arxiv.org/pdf/2401.01325) [[code](https://github.com/datamllab/LongLM): ![](https://img.shields.io/github/stars/datamllab/LongLM.svg?style=social)] | ZHongye Jin, Xiaotian Han, Jingfeng Yang, et. al. | Texas A&M University | <details><summary><small>This paper presents SelfExtend ...</small></summary><small>SelfExtend extend the context window of LLMs by construncting bi-level attention information without fine-tuning: 1) The grouped attention captures the dependencies amongo tokens that are far apart; 2) The neighbor attention captures dependencies among adjacent tokens within a specified range</small></details>|<sub>LongBench, L-Eval </sub>|
|2024/05/29 | [Beyond the Limits: A Survey of Techniques to Extend the Context Length in Large Language Models](https://arxiv.org/pdf/2402.02244) | Xindi Wang, Mahsa Salmani, Parsa Omidi, et. al. | Huawei Tech. Canada, University of Western Ontario | <details><summary><small>This paper presents a survey ...</small></summary><small>This paper survey works in enabling LLMs to handle long sequences, including *length extrapolation*, *attention approximation*, *attention-free transformers*, *model compression*, and *hardware-aware transformers*.</small></details>|<sub>None</sub>|

## 2. Haullucinations <a id="hallucinations"></a>

| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/09/13 | [Cognitive Mirage: A Review of Hallucinations in Large Language Models](https://arxiv.org/pdf/2309.06794.pdf) | Hongbin Ye, Tong Liu, Aijia Zhang, Wei Hua, Weiqiang Jia | Zhejiang Lab | <details><summary><small>This paper presents taxonomy of hallucinations ...</small></summary><small>This work provides a literature review on hallucinations, which presents a taxonomy of hallucinations from several text generation tasks, and mechanism analysis (three types: data collection, knowledge gap, and optimization process), detection methods and improvement approaches.</small></details>| <sub>-</sub>|

## 3. Datasets <a id="datasets"></a>

### 3.1 Factoid QA <a id="fqa"></a>

| Date       | Title | Authors   | Orgnization | Abs    | Dataset                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2024/01/26 | [Benchmarking Large Language Models in Complex Question Answering Attribution using Knowledge Graphs](https://arxiv.org/abs/2401.14640.pdf)| Nan Hu, Jiaoyan Chen, Yike Wu, Guilin Qi, Sheng Bi, Tongtong Wu, Jeff Z. Pan.|Southeast University, The University of Manchester,The University of Edinburgh |<details><summary><small>This paper presents CAQA ...</small></summary><small>CAQA is a new benchmark for complex question answering attribution, which is designed to evaluate the ability of LLMs to answer complex questions with the help of knowledge graphs.</small></details>| <sub> CAQA </sub>|
|2022/04/12| [ASQA: Factoid Questions Meet Long-Form Answers](https://arxiv.org/abs/2204.06092.pdf) [[dataset](https://huggingface.co/datasets/din0s/asqa)]|Ivan Stelmakh, Yi Luan, Bhuwan Dhingra, Ming-Wei Chang|Carnegie Mellon University, Duke University, Google Research |<details><summary><small>This paper presents ASQA ...</small></summary><small>ASQA is the first long-form question answering dataset that focuses on ambiguous factoid questions.</small></details>| <sub>ASQA</sub>|

### 3.2 Long-form QA <a id="lfqa"></a>

