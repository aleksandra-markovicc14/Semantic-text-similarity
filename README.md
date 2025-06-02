# Semantic-text-similarity

## Overview
This project focuses on predicting semantic similarity between pairs of sentences using the [STS Benchmark dataset](https://github.com/PhilipMay/stsb-multi-mt/tree/30de0dec4ee199b7f42351d3f1a0b19592955385/data). The dataset is composed of sentence pairs from domains such as news headlines, image captions, and user forums, each annotated with a similarity score ranging from 0 (no similarity) to 5 (identical meaning).

A variety of techniques were applied to this task:

- Unsupervised methods such as TF-IDF cosine similarity, n-gram extensions, and average word embedding distances
- Supervised models, both regression and classification-based, trained on sentence embeddings
- Transformer-based models were fine-tuned, including Sentence-BERT and variants

Model ensembling was performed using multiple pretrained models: 'all-MiniLM-L6-v2', 'all-mpnet-base-v2', 'all-roberta-large-v1', and 'msmarco-distilbert-base-v4' to improve robustness and accuracy

Additional datasets such as the [STS Companion]([tasksource/sts-companion](https://huggingface.co/datasets/mteb/stsbenchmark-sts)) and [SNLI corpus](https://nlp.stanford.edu/projects/snli/snli_1.0.zip) were incorporated to enhance model performance.

The workflow also included exploratory data analysis, similarity metric comparisons, and evaluation across model architectures


