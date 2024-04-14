# Awesome resources about intent understanding component in the RAG system

🔥 **Must-read papers for intent understanding component in RAG.**

🌟 **We greatly appreciate any contributions via PRs, issues, emails, or other methods.**


## Introduction

The intent understanding component is to understand the question, and guide the retrieval to obtain better documents. Usually, there could be different types of understanding, e.g., whether to retrieve and query formulations.


## Table of Content (ToC)

- [Retrieval Detection](#retrieval_detect)
- [Query Reformulation](#query_reformulate)


## 1. Retrieval Detection <a id="retrieval_detect"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|2023/10/08| [Self-Knowledge Guided Retrieval Augmentation for Large Language Models](https://arxiv.org/pdf/2310.05002.pdf) |Yile Wang, Peng Li, Maosong Sun, Yang Liu|Tsinghua University| <small>This work introduces Self-Knowledge guided Retrieval augmentation*SKR* to flexibly call the retriever. Three steps: 1) collection self-knowledge of LLM by asking a number of questions, and divide the question into two categories D+ and D- according to the answer correctness, 2) eliciting self-knowledge of LLMs by either direct prompt or training a classifier based on D+ and D-, 3) using self-knowledge for adaptive retrieval augmentation based on prediction of 2).</small>|

## 2. Query Reformulation <a id="query_reformulate"></a>

| Date       | Title                                                                                                           | Authors                                  | Orgnization                                                                                                   | Abs                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
