# TransformersFinalProject
Named Entity Recognition with BERT

## Project Proposal
#### Problem Statement:
The goal of this project is to develop a named entity recognition (NER) model using the pre-trained BERT model and fine-tune it on the CoNLL-2003 dataset to accurately identify and classify name
d entities in text.

#### Transformers and Datasets:
- Pre-trained BERT model: Leverages bidirectional architecture and self-attention mechanism to capture contextual information.
- Dataset used in this model is MIT Movie Corpus. The MIT Movie Corpus is a semantically tagged training and test corpus in BIO format. The eng corpus are simple queries, and the trivia10k13 corpus are more complex queries.
- https://groups.csail.mit.edu/sls/downloads/movie/

#### Revised Project Plan:
1. Input Collection:
   - Collect input text from the user to analyze for named entity recognition.
2. Tokenization and Encoding:
   - Use a tokenizer associated with a pre-trained BERT model to convert the input text into tokenized format suitable for model input. This includes encoding the text into a series of integers (tokens).
3. Loading the Pre-trained Model:
   - Load a pre-trained BERT model that is likely fine-tuned for a named entity recognition task.
4. Predicting Named Entities:
   - Use the model to predict entity labels for the tokenized text without further training. This step involves processing the input through the model and interpreting the output to obtain the most likely entity labels for each token.
5. Post-processing the Output:
   - Convert token IDs back to text tokens.
   - Merge subword tokens as necessary to align with typical word boundaries.
   - Convert predicted label indices back to label names using a predefined mapping (label dictionary).
6. Result Presentation:
   - Compile the tokens and their corresponding predicted labels into a structured format (e.g., a pandas DataFrame) and display the results in a user-friendly manner.