# Can Large Language Models Identify Authorship?

## Overview
This repository contains the code and data used in EMNLP 2024 Findings paper titled "Can Large Language Models Identify Authorship?" Our research focuses on exploring the capabilities of Large Language Models (LLMs) in authorship analysis tasks, specifically authorship verification and authorship attribution. The primary aim is to investigate whether LLMs can accurately identify the authorship of texts, which is pivotal for verifying content authenticity and mitigating misinformation.\
[[arXiv]](https://arxiv.org/pdf/2403.08213) [[Project Website]](https://llm-authorship.github.io/#canllm-identify-authorship)


As illustrated in figure below, LLMs correctly identifies that the two input texts are written by the same author and provides explanations. Linguistic features detected by the model are highlighted in different colors.
<img src="https://github.com/authorship-attribution-llm/authorship-llm-survey/blob/main/data/case.png" width=80%>


## BibTex
```
@artile{huang2024authorship,
    title   = {Can Large Language Models Identify Authorship?}, 
    author  = {Baixiang Huang and Canyu Chen and Kai Shu},
    year    = {2024},
    journal = {arXiv preprint},
    volume  = {abs/2403.08213},
    url     = {https://arxiv.org/abs/2403.08213}, 
}
```

## Methodology
Traditional authorship analysis methods rely on hand-crafted writing style features and classifiers, while state-of-the-art approaches utilize text embeddings from pre-trained language models, often requiring domain-specific fine-tuning. Our approach evaluates LLMs' performance in authorship analysis without the need for fine-tuning, and explores the integration of explicit linguistic features to enhance reasoning capabilities.

## Data Preprocessing
For this study, texts and authors were filtered to remove duplicates and authors contributing fewer than two texts. Non-English texts were excluded using the `py3langid` tool, available at [py3langid GitHub](https://github.com/adbar/py3langid).

## Datasets
The datasets used in this research are publicly available on Kaggle:
- Enron Email Dataset: [Access Here](https://www.kaggle.com/datasets/wcukierski/enron-email-dataset)
- Blog Authorship Corpus: [Access Here](https://www.kaggle.com/datasets/rtatman/blog-authorship-corpus)

## Code
The code accompanying this research is structured to facilitate the replication of our study and further exploration of LLMs in authorship analysis tasks. It includes scripts for data preprocessing and evaluation.


