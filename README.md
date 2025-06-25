A curated list of resources dedicated to retrieval-augmented generation (RAG).

The retrieval-augmented generation (RAG) is to combine the merits of retrieval system and llm to generation high-quality answers for users.


<div align="center">
    <img width="800" src="/assets/rag1.png" alt="RAG Framework">
    <br><br>
    <p><b>The Framework for RAG System</b></p>
</div>



Typically, the rag system consists of a set of modules, where each task are described as follows:
1. [Interpreter](/papers/interpreter/): This component focuses on refining and enriching the user's initial query or question to improve the subsequent retrieval process. By generating more detailed or expanded search queries, it helps the retrieval component to more effectively recall relevant documents.
2. [Retriever](/papers/retriever/): This component is responsible for finding and fetching relevant documents or passages from a large corpus based on the refined user query. It acts as the primary information access layer, providing the foundational knowledge for the generation phase. 
3. [Compressor](/papers/compressor/): This component processes the retrieved documents and user questions to create an optimized context for LLM. It aims to refine, condense, and organize the retrieved information, ensuring that the most pertinent and concise context is passed on for accurate generation. 
4. [Generator](/papers/generator/): This component leverages a LLM to synthesize a coherent, informative, and contextually relevant answer based on the user's question and the provided refined contexts. It transforms raw information into a human-readable response. 
5. [Validator](/papers/validator/): This component aims to improve the trustworthiness and quality of the generated answer by validating its accuracy and adherence to factual information within the provided contexts. It ensures the output is reliable and grounded.
6. [Evaluator](/papers/evaluator.md): This component measures the overall performance and quality of the RAG system, assessing various aspects such as answer accuracy, retrieval effectiveness, and generation faithfulness. It provides metrics to understand and improve the system's capabilities.

## Surveys

* The *Organization* column only record the organization of the first author.

| **Date** |                                                                        **Title**                                                                        |          **Organization**          |                                                                   **Code**                                                                   |
| :------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------: |
|   2024/09/16  |                              [Trustworthiness in Retrieval-Augmented Generation Systems: A Survey](https://arxiv.org/abs/2409.10102)                              |             Tsinghua University             |           [Code](https://github.com/smallporridge/TrustworthyRAG)<br>![](https://img.shields.io/github/stars/smallporridge/TrustworthyRAG.svg?style=social)           |
|   2024/09/10   |                              [Graph Retrieval-Augmented Generation: A Survey](https://arxiv.org/abs/2408.08921)                              |             Peking University             |           [Code](https://github.com/pengboci/GraphRAG-Survey)<br>![](https://img.shields.io/github/stars/pengboci/GraphRAG-Survey.svg?style=social)           |
|   2024/07/13   |                              [Large Language Models and Future of Information Retrieval: Opportunities and Challenges](https://dl.acm.org/doi/pdf/10.1145/3626772.3657848)                              |      ChengXiang Zhai, UIUC             |  -        |
|   2024/02/29   |                              [Retrieval-Augmented Generation for AI-Generated Content: A Survey](https://arxiv.org/abs/2402.19473)                              |             Peking University             |           [Code](https://github.com/hymie122/RAG-Survey)<br>![](https://img.shields.io/github/stars/hymie122/RAG-Survey.svg?style=social)           |
|   2024/01/03   |                              [Retrieval-Augmented Generation for Large Language Models: A Survey](https://arxiv.org/abs/2312.10997)                              |             Tongji University             |       [Code](https://github.com/Tongji-KGLLM/RAG-Survey)<br>![](https://img.shields.io/github/stars/Tongji-KGLLM/RAG-Survey.svg?style=social)       |
|   2024/01/03   |                    [A Comprehensive Survey of Hallucination Mitigation Techniques in Large Language Models](https://arxiv.org/abs/2401.01313)                    |     Islamic University of Technology     |                                                                         No                                                                         |
|   2023/12/07   | [Trends in Integration of Knowledge and Large Language Models: A Survey and Taxonomy of Methods, Benchmarks, and Applications](https://arxiv.org/abs/2311.05876) |      Harbin Institute of Technology      |                                                                         No                                                                         |
|   2023/09/19   |                            [The Rise and Potential of Large Language Model Based Agents: A Survey](https://arxiv.org/abs/2309.07864)                            |              Fudan NLP Group              | [Code](https://github.com/WooooDyy/LLM-Agent-Paper-List)<br>![](https://img.shields.io/github/stars/WooooDyy/LLM-Agent-Paper-List.svg?style=social) |
|   2023/08/14   |                                  [Large Language Models for Information Retrieval: A Survey](https://arxiv.org/abs/2308.07107)                                  |             Renmin University             |       [Code](https://github.com/RUC-NLPIR/LLM4IR-Survey)<br>![](https://img.shields.io/github/stars/RUC-NLPIR/LLM4IR-Survey.svg?style=social)       |
|   2022/02/02   |                                       [A Survey on Retrieval-Augmented Text Generation](https://arxiv.org/abs/2202.01110)                                       | Nara Institute of Science and Techonology |                                                                         No                                                                         |

## Systems

* The *Organization* column only record the organization of the first author.

| **Date** | **Title** | **Organization**  |  **Code**  |
| :-----------: | :-------------: | :----------------------: |  :----------------------: 
|2024/11/07|[LightRAG: Simple and Fast Retrieval-Augmented Generation](https://arxiv.org/abs/2410.05779)|BUPT|[Code](https://github.com/HKUDS/LightRAG)<br>![](https://img.shields.io/github/stars/HKUDS/LightRAG.svg?style=social)|
|2024/10/25|[StructRAG: Boosting Knowledge Intensive Reasoning of LLMs via Inference-time Hybrid Information Structurization](https://arxiv.org/abs/2410.08815)|ISCAS|[Code](https://github.com/Li-Z-Q/StructRAG)<br>![](https://img.shields.io/github/stars/Li-Z-Q/StructRAG.svg?style=social)|
|2024/08/21|[RAGLAB: A Modular and Research-Oriented Unified Framework for Retrieval-Augmented Generation](https://arxiv.org/abs/2408.11381)|Nanjing University|[Code](https://github.com/fate-ubw/RAGLab)<br>![](https://img.shields.io/github/stars/fate-ubw/RAGLab.svg?style=social)|
|2024/07/11|[Speculative RAG: Enhancing Retrieval Augmented Generation through Drafting](https://arxiv.org/abs/2407.08223)          |     University of California, San Diego     |        No        |
|2024/06/19|[InstructRAG: Instructing Retrieval-Augmented Generation via Self-Synthesized Rationales](https://arxiv.org/abs/2406.13629)|University of Virginia|[Code](https://github.com/weizhepei/InstructRAG)<br>![](https://img.shields.io/github/stars/weizhepei/InstructRAG.svg?style=social)|
|2024/05/22|[FlashRAG: A Modular Toolkit for Efficient Retrieval-Augmented Generation Research](https://arxiv.org/pdf/2405.13576)|Renmin University of China|[Code](https://github.com/RUC-NLPIR/FlashRAG)<br>![](https://img.shields.io/github/stars/RUC-NLPIR/FlashRAG.svg?style=social)|
|2024/04/24|[From Local to Global: A Graph RAG Approach to Query-Focused Summarization](https://arxiv.org/abs/2404.16130)               | Microsoft |     [Code](https://www.microsoft.com/en-us/research/project/graphrag/)     |
|2023/11/22|[FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation](https://arxiv.org/abs/2310.03214)|Google|[Code](https://github.com/freshllms/freshqa)<br>![](https://img.shields.io/github/stars/freshllms/freshqa.svg?style=social)|
|2023/11/08|[PDFTriage: Question Answering over Long, Structured Documents](https://arxiv.org/abs/2309.08872)|Stanford|[Code](https://github.com/HAMNET-AI/PDFTriage)<br>![](https://img.shields.io/github/stars/HAMNET-AI/PDFTriage.svg?style=social)|
|2023/10/27|[WikiChat: Stopping the Hallucination of Large Language Model Chatbots by Few-Shot Grounding on Wikipedia](https://arxiv.org/pdf/2305.14292v2.pdf)|Stanford|[Code](https://github.com/stanford-oval/WikiChat)<br>![](https://img.shields.io/github/stars/stanford-oval/WikiChat.svg?style=social)|
|2023/10/27|[LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://arxiv.org/abs/2306.15626)|Caltech|[Code](https://github.com/lean-dojo/LeanDojo)<br>![](https://img.shields.io/github/stars/lean-dojo/LeanDojo.svg?style=social)|
|2023/06/13|[WebGLM: Towards An Efficient Web-Enhanced Question Answering System with Human Preferences](https://arxiv.org/abs/2306.07906)|Tsinghua University|[Code](https://github.com/THUDM/WebGLM)<br>![](https://img.shields.io/github/stars/THUDM/WebGLM.svg?style=social)|
|2023/05/23|[WebCPM: Interactive Web Search for Chinese Long-form Question Answering](https://arxiv.org/abs/2305.06849)|Tsinghua University|[Code](https://github.com/thunlp/WebCPM)<br>![](https://img.shields.io/github/stars/thunlp/WebCPM.svg?style=social)|
|2022/06/01|[WebGPT: Browser-assisted question-answering with human feedback](https://arxiv.org/abs/2112.09332)|Open AI|No|


