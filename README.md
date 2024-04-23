# TransformersFinalProject
Named Entity Recognition with BERT


## Requirements
```bash
pip install transformers sklearn tensorflow
```

## Project Proposal
#### Problem Statement:
The goal of this project is to develop a named entity recognition (NER) model using the pre-trained BERT model and fine-tune it on the CoNLL-2003 dataset to accurately identify and classify name
d entities in text.

#### Transformers and Datasets:
- Pre-trained BERT model: Leverages bidirectional architecture and self-attention mechanism to capture contextual information.
- Dataset used in this model is MIT Movie Corpus. The MIT Movie Corpus is a semantically tagged training and test corpus in BIO format. The eng corpus are simple queries, and the trivia10k13 corpus are more complex queries.
- https://groups.csail.mit.edu/sls/downloads/movie/

#### Project Plan:
1. Preprocess the data by tokenizing the input text and aligning entity labels with the tokenized text.
2. Load the pre-trained BERT model and add a token-level classification layer on top.
3. Fine-tune the BERT model on the MIT Movie Corpus dataset using prepared input sequences and entity labels.
4. Evaluate the fine-tuned model on the test set using precision, recall, and F1-score metrics.
5. Experiment with different input formats, fine-tuning strategies, and compare performance with other models.