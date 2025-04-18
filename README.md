# Awesome GraphRAG
<div align="center">
    <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/AwesomeGraphRAG-welcome-red.svg"/></a>
    <a href="http://makeapullrequest.com"><img src="https://img.shields.io/github/stars/SJTU-DMTai/awesome-rag"/></a>
</div>
<div align="center">
  This repository contains a curated list of resources on graph-based RAG methods. 
</div>
<div align="center">
    Continuously updating, stay tuned!
</div>

# Introduction
**Large language models (LLMs)** have demonstrated remarkable capabilities across diverse tasks, achieving significant advancements in text comprehension, question answering, and content generation. However, their performance in knowledge-intensive tasks, particularly those requiring domain expertise, remains suboptimal due to the folllowing limitations: their pretrained knowledge, though broad, lacks depth in specialized areas due to reliance on general-domain data, resulting in inconsistencies with current domain standards; they struggle with precise, multi-step reasoning required by domain-specific rules, often failing to maintain logical consistency and accuracy in complex reasoning chains; and they exhibit limited context sensitivity, frequently misinterpreting or oversimplifying domain-specific terms and concepts that vary meaning based on context.

**Retrieval-Augmented generation (RAG)** offers a promising solution to customize LLMs for specific domains. Rather than retraining LLMs to incorporate updates, RAG enhances these models by leveraging external knowledge from text corpora without modifying their architecture or parameters. This approach enables LLMs to generate responses by leveraging not only their pre-trained knowledge but also real-time retrieved domain-specific information, thereby providing more accurate and reliable answers. However, the practical effectiveness of RAG systems in real-world applications is hindered by limitations in complex query comprehension, difficulties in synthesizing distributed domain knowledge, inherent constraints of LLMs, and issues with system efficiency and scalability[1].

To address these limitations, **graph retrieval-augmented generation (GraphRAG)** has recently emerged as a new paradigm to customize LLMs with well-organized background knowledge and improved contextual reasoning. GraphRAG, formally defined as a specialized subclass of the RAG framework, utilizes graph structures to systematically organize and retrieve domain-specific knowledge. Its workflow encompasses two key stages: offline indexing and online retrieval. The overall pipeline is as follows.
![pipeline_v2.png](pipeline_v3.png)
We collect the recent influential papers and benchmarks about GraphRAG. The following contents are listed in chronological order of publication.


# 📑 Research Paper
|Date|Venue|Title|Code|Notes|
|:---:|:---:|:---:|:---:|:---:|
|2025-03-18|Arxiv|[KG-IRAG: A Knowledge Graph-Based Iterative Retrieval-Augmented Generation Framework for Temporal Reasoning](https://arxiv.org/abs/2503.14234)|No|*Graphs for Knowledge Indexing & Graphs as Knowledge Carrier(KG construction from corpus)*|
|2025-03-13|Arxiv|[Retrieval-Augmented Generation with Hierarchical Knowledge](https://arxiv.org/abs/2503.10150)|[Yes](https://github.com/hhy-huang/HiRAG)|*Graphs for Knowledge Indexing & Graphs as Knowledge Carrier(KG construction from corpus)*|
|2025-03-06|Arxiv|[In-depth Analysis of Graph-based RAG in a Unified Framework](https://arxiv.org/abs/2503.04338)|[Yes](https://github.com/JayLZhou/GraphRAG)|*modularizing and decoupling some graph-based RAG methods to unveil the mystery behind them and share fun and valuable insights!*|
|2025-02-20|Arxiv|[(HippoRAG 2)From RAG to Memory: Non-Parametric Continual Learning for Large Language Models](https://arxiv.org/abs/2502.14802)|[Yes](https://github.com/OSU-NLP-Group/HippoRAG)|*Graphs for Knowledge Indexing & Graphs as Knowledge Carrier(KG construction from corpus)*|
|2025-02-14|Arxiv|[ArchRAG: Attributed Community-based Hierarchical Retrieval-Augmented Generation](https://arxiv.org/abs/2502.09891)|No|*Graphs for Knowledge Indexing & Graphs as Knowledge Carrier(KG construction from corpus)*|
|2025-02-08|NAACL 2025|[(KG2RAG)Knowledge Graph-Guided Retrieval Augmented Generation](https://arxiv.org/abs/2502.06864)|[Yes](https://github.com/nju-websoft/KG2RAG)|*Graphs for Knowledge Indexing & Graphs as Knowledge Carrier(KG construction from corpus)*|
|2025-02-06|The ACM Web Conference 2025|[MedRAG: Enhancing Retrieval-augmented Generation with Knowledge Graph-Elicited Reasoning for Healthcare Copilot](https://arxiv.org/abs/2502.04413)|[Yes](https://github.com/SNOWTEAM2023/MedRAG?tab=readme-ov-file)|*Graphs as Knowledge Carrier(KG construction from corpus)*|
|2024-12-17|Arxiv|[SimGRAG: Leveraging Similar Subgraphs for Knowledge Graphs Driven Retrieval-Augmented Generation](https://arxiv.org/abs/2412.15272)|[Yes](https://github.com/YZ-Cai/SimGRAG)|*Graphs as Knowledge Carrier(KG construction from corpus & with existing KGs)*|
|2024-10-28|ICLR 2025|[Simple Is Effective: The Roles of Graphs and Large Language Models in Knowledge-Graph-Based Retrieval-Augmented Generation](https://arxiv.org/abs/2410.20724)|[Yes](https://github.com/Graph-COM/SubgraphRAG)|*Graphs as Knowledge Carrier(KG construction from corpus)*|
|2024-10-08|Arxiv|[LightRAG: Simple and Fast Retrieval-Augmented Generation](https://arxiv.org/abs/2410.05779)|[Yes](https://github.com/HKUDS/LightRAG)|*Graphs as Knowledge Carrier(KG construction from corpus)*|
|2024-05-23|NeurIPS 2024|[HippoRAG: Neurobiologically Inspired Long-Term Memory for Large Language Models](https://arxiv.org/abs/2405.14831)|[Yes](https://github.com/OSU-NLP-Group/HippoRAG)|*Graphs as Knowledge Carrier(KG construction from corpus)*|
|2024-04-24|Arxiv|[From Local to Global: A Graph RAG Approach to Query-Focused Summarization](https://arxiv.org/abs/2404.16130)|[Yes](https://github.com/microsoft/graphrag)|*Graphs as Knowledge Carrier(Knowledge Graph Construction from Corpus)*|


# 🔥 Hot Methods
|Date|Method|Graph Type|Index Component|Retrieval Primitive|Retrieval Granularity|Code|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|2024-10-31|[fast-graphrag](https://github.com/circlemind-ai/fast-graphrag?tab=readme-ov-file)|Textual Knowledge Graph|Entity|Entities in question|Entity, Relationship, Chunk|[Yes](https://github.com/circlemind-ai/fast-graphrag?tab=readme-ov-file)|
|2024-10-08|[LightRAG_Local](https://arxiv.org/abs/2410.05779)|Rich Knowledge Graph|Entity, Relationship|Low-level keywords in question|Entity, Relationship, Chunk|[Yes](https://github.com/hkuds/lightrag)|
|2024-10-08|[LightRAG_Global](https://arxiv.org/abs/2410.05779)|Rich Knowledge Graph|Entity, Relationship|High-level keywords in question|Entity, Relationship, Chunk|[Yes](https://github.com/hkuds/lightrag)|
|2024-10-08|[LightRAG_Hybrid](https://arxiv.org/abs/2410.05779)|Rich Knowledge Graph|Entity, Relationship|Both high- and low-level keywords|Entity, Relationship, Chunk|[Yes](https://github.com/hkuds/lightrag)|
|2024-05-23|[HippoRAG](https://arxiv.org/abs/2405.14831)|Knowledge Graph|Entity|Entities in question|Chunk|[Yes](https://github.com/OSU-NLP-Group/HippoRAG)|
|2024-04-24|[GraphRAG_Local](https://arxiv.org/abs/2404.16130)|Textual Knowledge Graph|Entity, Community|Question vector|Entity, Relationship, Chunk, Community|[Yes](https://github.com/microsoft/graphrag)|
|2024-04-24|[GraphRAG_Global](https://arxiv.org/abs/2404.16130)|Textual Knowledge Graph|Community|Question vector|Community|[Yes](https://github.com/microsoft/graphrag)|
|2024-01-31|[RAPTOR](https://arxiv.org/abs/2401.18059)|Tree|Tree node|Question vector|Tree node|[Yes](https://github.com/parthsarthi03/RAPTOR)|

Note: This repo summarizes the graph constructed from the corpus into the following categories according to [2]:
1. **Passage Graph**: each chunk represents a node. If two chunks contain a number of the same entities larger than a threshold, link an edge for these two nodes.
2. **Tree**: a tree is built progressively by clustering leaf nodes at each layer and using an LLM to generate higher-level summary nodes for clusters with multiple children.
3. **Knowledge Graph**: extracting entities and relationships from each chunk
4. **Textual Knowledge Graph**: a specialized KG    , with the key difference being that in a TKG, each entity and relationship is assigned a brief textual description.
5. **Rich Knowledge Graph**: an extended version of TKG, containing more information, including textual descriptions for entities and relationships, as well as keywords for relationships.


# 🧐 Survey Papers
|Date|Venue|Title|Repo|
|:---:|:---:|:---:|:---:|
|2025-01-21|Arxiv|[A Survey of Graph Retrieval-Augmented Generation for Customized Large Language Models](https://arxiv.org/abs/2501.13958)|[Yes](https://github.com/DEEP-PolyU/Awesome-GraphRAG)|
|2024-12-31|Arxiv|[Retrieval-Augmented Generation with Graphs (GraphRAG)](https://arxiv.org/abs/2501.00309))|[Yes](https://github.com/Graph-RAG/GraphRAG/)|
|2024-08-15|Arxiv|[Graph Retrieval-Augmented Generation: A Survey](https://arxiv.org/abs/2408.08921)|[Yes](https://github.com/pengboci/GraphRAG-Survey)|
|2024-05-10|KDD 2024|[A Survey on RAG Meeting LLMs: Towards Retrieval-Augmented Large Language Models](https://arxiv.org/abs/2405.06211)|No|


# 🥇 Benchmark
|Dataset|Task|Info|Metrix|
|:---:|:---:|:---:|:---:|
|[NaturalQuestions](https://ai.google.com/research/NaturalQuestions)|Simple QA|A general-domain simple QA dataset based on the Wikipedia dump knowledge base, testing the model’s ability to extract answers from encyclopedia content.|EM, F1 Score|
|[PopQA](https://huggingface.co/datasets/akariasai/PopQA)|Simple QA|PopQA is a large-scale open-domain question answering (QA) dataset, consisting of 14k entity-centric QA pairs. Each question is created by converting a knowledge tuple retrieved from Wikidata using a template. Each question come with the original subject_entitiey, object_entityand relationship_type annotation, as well as Wikipedia monthly page views.|Accuracy, F1 Score|
|[SimpleQuestion](https://huggingface.co/datasets/fbougares/simple_questions_v2/)|Simple QA|SimpleQuestions is a large-scale factoid question answering dataset. It consists of 108,442 natural language questions, each paired with a corresponding fact from Freebase knowledge base. Each fact is a triple (subject, relation, object) and the answer to the question is always the object.|EM, F1 Score|
|[WebQ](https://huggingface.co/datasets/Stanford/web_questions)|Simple QA|This dataset consists of 6,642 question/answer pairs. The questions are supposed to be answerable by Freebase, a large knowledge graph. The questions are mostly centered around a single named entity.|Precision, Recall|
|[WebQSP](https://www.microsoft.com/en-us/download/details.aspx?id=52763)|Simple QA|A general simple QA dataset finishing semantic parsing and QA tasks based on Freebase.|EM|
|[MuSiQue](https://github.com/StonyBrookNLP/musique)|Multi-hop QA|A general multi-hop QA dataset with implicit in-data knowledge, testing multi-step reasoning ability.|answer_f1, support_f1|
|[2WikiMultihopQA](https://github.com/Alab-NII/2wikimultihop)|Multi-hop QA|A general multi-hop QA dataset with in-data implicit knowledge, emphasizing cross-Wikipedia paragraph reasoning.|EM, F1 Score|
|[HotpotQA](https://hotpotqa.github.io/)|Multi-hop QA|A question answering dataset featuring natural, multi-hop questions, with strong supervision for supporting facts to enable more explainable question answering systems based on Wikipedia dump.|EM, F1 Score, Accuracy, Recall|
|[CWQ](https://huggingface.co/datasets/drt/complex_web_questions)|Multi-hop QA|A dataset for answering complex questions that require reasoning over multiple web snippets via Freebase.|Accuracy|
|[MultiHop-RAG](https://github.com/yixuantt/MultiHop-RAG/)|Multi-hop QA|A Dataset for Evaluating Retrieval-Augmented Generation Across Documents.|Hits@10, Hits@4, MAP@10, MRR@10, Accuracy, Recall|
|[MetaQA](https://github.com/yuyuz/MetaQA)|Multi-hop QA|A movie-domain multi-hop QA dataset relying on the in-data movie knowledge base for reasoning.|Accuracy|
|[Mintaka](https://huggingface.co/datasets/AmazonScience/mintaka)|Complex QA|Mintaka is a complex, natural, and multilingual question answering (QA) dataset composed of 20,000 question-answer pairs elicited from MTurk workers and annotated with Wikidata question and answer entities.|EM, F1 Score, Hits@1|
|[GrailQA](https://dki-lab.github.io/GrailQA/)|Complex QA|A a new large-scale, high-quality dataset for question answering on knowledge bases (KBQA) on Freebase with 64,331 questions annotated with both answers and corresponding logical forms in different synta|Accuracy|
|[UltraDomain](https://huggingface.co/datasets/TommyChien/UltraDomain)|Complex QA|An 18-domain complex QA dataset testing cross-domain complex question-handling ability.|LLM as judger, like GraphRAG & LightRAG|
|[TriviaQA](https://huggingface.co/datasets/mandarjoshi/trivia_qa)|Complex QA|TriviaqQA is a reading comprehension dataset containing over 650K question-answer-evidence triples. TriviaqQA includes 95K question-answer pairs authored by trivia enthusiasts and independently gathered evidence documents, six per question on average, that provide high quality distant supervision for answering the questions.|Accuracy|
|[LC-QuAD v2](https://huggingface.co/datasets/mohnish/lc_quad)|Complex QA|LC-QuAD 2.0 is a Large Question Answering dataset with 30,000 pairs of question and its corresponding SPARQL query. The target knowledge base is Wikidata and DBpedia, specifically the 2018 version.|Accuracy|
|[KQAPro](https://huggingface.co/datasets/drt/kqa_pro)|Large-scale Complex QA|A large-scale dataset of complex question answering over Wikidata. The questions are very diverse and challenging, requiring multiple reasoning capabilities including compositional reasoning, multi-hop reasoning, quantitative comparison, set operations, and etc.|Accuracy|
|[FACTKG](https://github.com/jiho283/FactKG?tab=readme-ov-file)|Fact Verification|Fact Verification via Reasoning on Knowledge Graphs. It consists of 108k natural language claims with five types of reasoning: One-hop, Conjunction, Existence, Multi-hop, and Negation based on DBpedia.|Accuracy|
|[DDXPlus](https://github.com/mila-iqia/ddxplus)|Medical QA & Diagnostic support|A new large-scale dataset for Automatic Symptom Detection (ASD) and Automatic Diagnosis (AD) systems in the medical domain.|IL (Interaction Length), GTPA (Ground Truth Probability Above Threshold), DDR/DDP/DDF1 (Differential Diagnosis Recall/Precision/F1), DSP/DSR/DSF1 (Severity Precision/Recall/F1)|
|[NarrativeQA](https://huggingface.co/datasets/deepmind/narrativeqa)|QA & **Discourse Understanding**|An English-lanaguage dataset of stories and corresponding questions designed to test reading comprehension, especially on long documents.|BLEU, MET, ROU|


# 📊 Existing Knowledge Graphs
|Date|Venue|Title|Homepage|Domain|
|:------:|:---:|:---:|:---:|:---:|
|2023-08-23|SIGIR 2024|[YAGO 4.5: A Large and Clean Knowledge Base with a Rich Taxonomy](https://arxiv.org/abs/2308.11884)|[Yes](https://yago-knowledge.org/)|General|
|2023-02-09|Bioinformatics|[The scalable precision medicine open knowledge engine (spoke): a massive knowledge graph of biomedical information](https://academic.oup.com/bioinformatics/article/39/2/btad080/7033465?login=false)|[Yes](https://spoke.ucsf.edu/)|Biomedical|
|2018-11-22|Nucleic acids research|[String v11: protein–protein association networks with increased coverage, supporting functional discovery in genome-wide experimental datasets](https://academic.oup.com/nar/article/47/D1/D607/5198476?login=false)|[Yes](https://string-db.org/)|Protein-protein interaction prediction|
|2018-05-12|LREC workshop|[Lynx: building the legal knowledge graph for smart compliance services in multilingual europe](http://lrec-conf.org/workshops/lrec2018/W22/pdf/12_W22.pdf)|[Yes](https://lynx-project.eu/)|Legal|


# ✅ Citation
- [1] A Survey of Graph Retrieval-Augmented Generation  for Customized Large Language Models.
- [2] In-depth Analysis of Graph-based RAG in a Unified Framework.
