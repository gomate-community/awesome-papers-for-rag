# awesome-papers-for-rag
A curated list of resources dedicated to retrieval-augmented generation (RAG).

The retrieval-augmented generation (RAG) is to combine the merits of retrieval system and llm to generation high-quality answers for users.

<div align="center">
    <img width="500" src="./rag.png" alt="RAG Framework">
    <br><br>
    <p><b>The Framework for RAG System</b></p>
</div>


Typically, the rag system consists of a set of modules, where each task are described as follows:

|                                          **Sub-Tasks**                                           | **Input** |     **Output**      |
| :------------------------------------------------------------------------------------------: | :-------------: | :----------------------: |
| [query understand](./query_understand.md) |      question      | search queries |
| [document retrieval](./searcher.md) |    question/queries     |     documents     |
| [evidence extraction](./compressor.md) |     questions+documents     |         contexts          |
| [answer generation](./generator.md)   |    question+contexts    |         answer |
| [result validation](./validator.md)   |    question+answer+contexts    |     True/False  |

### Healthcheck

```python
pip3 install -r requirements.txt
python3 healthcheck.py
```

### Survey Papers for RAG
* The *Organization* column only record the organization of the first author.

| **Date** | **Title** | **Organization**  |  **Code**  |
| :-----------: | :-------------: | :----------------------: |  :----------------------: |
|2024/01/03| [Retrieval-Augmented Generation for Large Language Models: A Survey](https://arxiv.org/abs/2312.10997)|Tongji University|[Code](https://github.com/Tongji-KGLLM/RAG-Survey)<br>![](https://img.shields.io/github/stars/Tongji-KGLLM/RAG-Survey.svg?style=social)|
|2024/01/03|[A Comprehensive Survey of Hallucination Mitigation Techniques in Large Language Models](https://arxiv.org/abs/2401.01313)|Islamic University of Technology|No|
|2023/09/19|[The Rise and Potential of Large Language Model Based Agents: A Survey](https://arxiv.org/abs/2309.07864)|Fudan NLP Group|[Code](https://github.com/WooooDyy/LLM-Agent-Paper-List)<br>![](https://img.shields.io/github/stars/WooooDyy/LLM-Agent-Paper-List.svg?style=social)|
|2023/08/14|[Large Language Models for Information Retrieval: A Survey](https://arxiv.org/abs/2308.07107)|Renmin University|[Code](https://github.com/RUC-NLPIR/LLM4IR-Survey)<br>![](https://img.shields.io/github/stars/RUC-NLPIR/LLM4IR-Survey.svg?style=social)|


### System Papers for RAG
* The *Organization* column only record the organization of the first author.

| **Date** | **Title** | **Organization**  |  **Code**  |
| :-----------: | :-------------: | :----------------------: |  :----------------------: |
|2023/11/22|[FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation](https://arxiv.org/abs/2310.03214)|Google|[Code](https://github.com/freshllms/freshqa)<br>![](https://img.shields.io/github/stars/freshllms/freshqa.svg?style=social)|
|2023/11/08|[PDFTriage: Question Answering over Long, Structured Documents](https://arxiv.org/abs/2309.08872)|Stanford|[Code](https://github.com/HAMNET-AI/PDFTriage)<br>![](https://img.shields.io/github/stars/HAMNET-AI/PDFTriage.svg?style=social)|
|2023/10/27|[WikiChat: Stopping the Hallucination of Large Language Model Chatbots by Few-Shot Grounding on Wikipedia](https://arxiv.org/pdf/2305.14292v2.pdf)|Stanford|[Code](https://github.com/stanford-oval/WikiChat)<br>![](https://img.shields.io/github/stars/stanford-oval/WikiChat.svg?style=social)|
|2023/10/27|[LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://arxiv.org/abs/2306.15626)|Caltech|[Code](https://github.com/lean-dojo/LeanDojo)<br>![](https://img.shields.io/github/stars/lean-dojo/LeanDojo.svg?style=social)|
|2023/06/13|[WebGLM: Towards An Efficient Web-Enhanced Question Answering System with Human Preferences](https://arxiv.org/abs/2306.07906)|Tsinghua University|[Code](https://github.com/THUDM/WebGLM)<br>![](https://img.shields.io/github/stars/THUDM/WebGLM.svg?style=social)|
|2023/05/23|[WebCPM: Interactive Web Search for Chinese Long-form Question Answering](https://arxiv.org/abs/2305.06849)|Tsinghua University|[Code](https://github.com/thunlp/WebCPM)<br>![](https://img.shields.io/github/stars/thunlp/WebCPM.svg?style=social)|
|2022/06/01|[WebGPT: Browser-assisted question-answering with human feedback](https://arxiv.org/abs/2112.09332)|Open AI|No|