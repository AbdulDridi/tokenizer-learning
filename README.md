# tokenizer-learning

A simple repository for learning about tokenizers by implementing them from scratch.


Tokenization is a text specific task that converts a sequence of characters into a sequence of tokens. Tokens are discrete units that represent text and can map to words, subwords, or characters, depending on the tokenizer.

This is a crucial initial step in many NLP tasks, including the use and training of large language models (LLMs). This is because the core gradient-based optimization algorithms used in training LLMs (such as gradient descent and backpropagation) operate in continuous vector space, and tokenization is the initial step in a process that converts text into a format suitable for these algorithms (the next step in the process being embedding the tokens into continuous vector space).

The repository contains step-by-step implementations of various tokenization algorithms, including:

[BPE (Byte Pair Encoding)](./bpe/README.md): A widely used two-stage algorithm introduced to the LLM domain by the [GPT-2 Paper](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf). The first builds a vocabulary of frequent subword units. Once this is built, the vocabulary is used to tokenize text 