# AgriLens: Semantic Retrieval in Agricultural Texts Using Topic Modeling and Language Models
## [ENAGRINEWS Dataset](https://www.researchsquare.com/article/rs-3107561/v1)


## Abstract
As the volume of unstructured text continues to grow across domains, there is an urgent need for scalable
methods that enable interpretable organization, summarization, and retrieval of information. This work presents
a unified framework for interpretable topic modeling, zero-shot topic labeling, and topic-guided semantic retrieval
over large agricultural text corpora. Leveraging BERTopic, we extract semantically coherent topics. Each topic is
converted into a structured prompt, enabling a language model to generate meaningful topic labels and summaries
in a zero-shot manner. Querying and document exploration are supported via dense embeddings and vector search,
while a dedicated evaluation module assesses topical coherence and bias. This framework supports scalable and
interpretable information access in specialized domains where labeled data is limited.

---

## Publication
This work is published in the  
**32nd IEEE International Conference on High Performance Computing, Data, and Analytics (HiPC)**  
Workshop Track: *Democratizing GenAI and Scalable NLP with HiPC for Societal Impact*  


---

## Dataset 📄
We use the [ENAGRINEWS Dataset](https://www.researchsquare.com/article/rs-3107561/v1),  
an open-access agricultural news corpus containing over 22,000 documents collected between 2020 and 2022.

---

## Code
All code to reproduce the experiments and framework described in the paper is available in this repository.  
Key components include:
- Topic Modeling with BERTopic  
- Zero-Shot Topic Labeling  
- Semantic Retrieval using dense embeddings + vector search  
- Evaluation of topical coherence and bias  

---

## Citation
If you use this framework or dataset in your research, please cite:

