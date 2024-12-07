# Awesome RAG Papers
This is a repo contains a list of papers about RAG, especially RAG with Knowledge Graphs

# Introduction
**Large language models (LLMs)** have demonstrated impressive reasoning abilities in complex tasks. However, they lack up-to-date knowledge and experience hallucinations during reasoning, which can lead to incorrect reasoning processes and diminish their performance and trustworthiness.

Recently, **Retrieval-Augmented Generation (RAG)** has achieved remarkable success in addressing the challenges of LLMs without necessitating retraining. By referencing an external knowledge base, RAG refines LLM outputs, effectively mitigating issues such as “hallucination”, lack of domain-specific knowledge, and outdated information. But in some practical scenarios, traditional RAG fails to capture significant structured relational knowledge, often recounts content in the form of text when concatenated as prompts and fails to grasp global information comprehensively.

Combining RAG with **Knowledge Graphs (KGs)** emerges as a promising solution to address these challenges. KGs can offer a structured and explicit representation of entities and relationships that are more accurate than retrieving information through vector similarity. Leveraging external structured knowledge graphs can improve contextual understanding of LLMs and generate more informed responses. The entire process typically contains three stages: Indexing, Retrieval and Generation. The overall pipline is as follows.

Pic needed to add...coming soon...

We collect the recent influential papers about RAG especially RAG with KGs. The following papers are listed in chronological order of publication.


# Paper List
## 2024
|Date|Venue|Title|Code|Description|
|:-----:|:------:|:------------:|:----:|:-----:|
|2024-02-06|ICML 24|[DFA-RAG: Conversational Semantic Router for Large Language Model with Definite Finite Automaton](https://arxiv.org/abs/2402.04411)|No||
|2024-02-12|Arxiv|[G-Retriever: Retrieval-Augmented Generation for Textual Graph Understanding and Question Answering](https://arxiv.org/abs/2402.07630)|[Yes](https://github.com/xiaoxinhe/g-retriever)|
|2024-02-19|Arxiv|[Graph-Based Retriever Captures the Long Tail of Biomedical Knowledge](https://arxiv.org/abs/2402.12352)|No|
|2024-03-09|Arxiv|[KG-Rank: Enhancing Large Language Models for Medical QA with Knowledge Graphs and Ranking Techniques](https://arxiv.org/abs/2403.05881)|[Yes](https://github.com/yangrui525/kg-rank)|
|2024-04-10|Arxiv|[Graph Chain-of-Thought: Augmenting Large Language Models by Reasoning on Graphs](https://arxiv.org/abs/2404.07103)|[Yes](https://github.com/PeterGriffinJin/Graph-CoT)|
|2024-04-24|Arxiv|[From Local to Global: A Graph RAG Approach to Query-Focused Summarization](https://arxiv.org/abs/2404.16130)|[Yes](https://github.com/microsoft/graphrag)|*This paper propose a two-stage approach using a large language model (LLM) to build a graph-based text index: first, deriving an entity knowledge graph from source documents, and second, pre-generating community summaries for closely-related entities. When a question is posed, each community summary generates a partial response, which are then summarized into a final user response.*|
|2024-04-26|SIGIR 2024|[Retrieval-Augmented Generation with Knowledge Graphs for Customer Service Question Answering](https://arxiv.org/abs/2404.17723)|No|
|2024-05-08|EMNLP 2024|[DALK: Dynamic Co-Augmentation of LLMs and KG to answer Alzheimer's Disease Questions with Scientific Literature](https://arxiv.org/abs/2405.04819)|[Yes](https://github.com/david-li0406/dalk)|
|2024-05-10|KDD 24|[A Survey on RAG Meeting LLMs: Towards Retrieval-Augmented Large Language Models](https://arxiv.org/abs/2405.06211)|No|
|2024-05-13|Arxiv|[Evaluation of Retrieval-Augmented Generation: A Survey](https://arxiv.org/abs/2405.07437)|[Yes](https://github.com/yhpeter/awesome-rag-evaluation)|
|2024-05-20|Arxiv|[KG-RAG: Bridging the Gap Between Knowledge and Creativity](https://arxiv.org/abs/2405.12035)|[Yes](https://github.com/BaranziniLab/KG_RAG)|
|2024-05-23|Arxiv|[HippoRAG: Neurobiologically Inspired Long-Term Memory for Large Language Models](https://arxiv.org/abs/2405.14831)|[Yes](https://github.com/OSU-NLP-Group/HippoRAG)|*Need to review*|
|2024-05-26|Arxiv|[GRAG: Graph Retrieval-Augmented Generation](https://arxiv.org/abs/2405.16506)|No|
|2024-07-20|Arxiv|[Golden-Retriever: High-Fidelity Agentic Retrieval Augmented Generation for Industrial Knowledge Base](https://arxiv.org/abs/2408.00798)|No|
|2024-08-09|Arxiv|[HybridRAG: Integrating Knowledge Graphs and Vector Retrieval Augmented Generation for Efficient Information Extraction](https://arxiv.org/abs/2408.04948)|No|
| 2024-08-15 | Arxiv | [Graph Retrieval-Augmented Generation: A Survey](https://arxiv.org/abs/2408.08921)| No |*This paper provides an overview of GraphRAG, a methodology that enhances language models by integrating knowledge graphs to improve retrieval accuracy and contextual responses. It details the GraphRAG workflow, from indexing to retrieval and generation, and discusses its applications and future research directions, highlighting its potential across various domains.*|
|2024-10-08|Arxiv|[LightRAG: Simple and Fast Retrieval-Augmented Generation](https://arxiv.org/abs/2410.05779)|[Yes](https://github.com/HKUDS/LightRAG)|*This paper proposes a system that integrates graph structures into text indexing and retrieval to address the limitations of existing RAG systems in handling complex interdependencies between entities. The system includes an incremental update algorithm to ensure timely integration of new data, keeping the system effective in rapidly changing data environments.*|

## 2023
|Date|Venue|Title|Code|Description|
|:-----:|:------:|:------------:|:----:|:-----:|
|2023-10-17|ICLR 24|[Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection](https://arxiv.org/abs/2310.11511)|[Yes](https://github.com/AkariAsai/self-rag)|
|2023-12-05|Arxiv|[Large Language Models on Graphs: A Comprehensive Survey](https://arxiv.org/abs/2312.02783)|No|
|2023-12-11|Arxiv|[KnowGPT: Knowledge Graph based Prompting for Large Language Models](https://arxiv.org/abs/2312.06185)|No|
|2023-12-18|Arxiv|[Retrieval-Augmented Generation for Large Language Models: A Survey](https://arxiv.org/abs/2312.10997)|No|*The survey outlines the evolution of RAG through three paradigms: Naive RAG, Advanced RAG, and Modular RAG. It meticulously examines the three foundational components of RAG frameworks, which include retrieval, generation, and augmentation techniques. The paper highlights the state-of-the-art technologies embedded in each of these components, offering a profound understanding of the advancements in RAG systems.*|

## Benchmark
|Date|Venue|Title|Code|Description|
|:-----:|:------:|:------------:|:----:|:-----:|
|2024-06-07|NeurIPS 2024|[CRAG -- Comprehensive RAG Benchmark](https://arxiv.org/abs/2406.04744)|[Yes](https://github.com/facebookresearch/crag)|*CRAG is designed to encapsulate a diverse array of questions across five domains and eight question categories, reflecting varied entity popularity from popular to long-tail, and temporal dynamisms ranging from years to seconds*|
