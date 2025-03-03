# thai-tokenizer-evaluations

This project is an extension of a previous analysis focused on Thai word segmentation algorithms, aimed at determining word boundaries in Thai text. Since languages like Thai do not use spaces to delimit words, this project is essential for enabling various natural language processing tasks, including part-of-speech tagging, language translation, and text-to-speech (TTS) conversion.

## Overview

The project combines linguistic analysis with the implementation of Python scripts to process a dataset and evaluate the performance of a Thai language library, PyThaiNLP. This analysis focuses on several aspects of text processing, including:

1. Word Tokenization
2. Sentence Tokenization
3. Spellcheck
4. Named Entity Recognition (NER)
5. Speed Test Evaluation

## Implementation

### Tools and Libraries

- Python: The programming language used for analysis and implementation.
- PyThaiNLP: A Thai NLP library that provides various tools and algorithms for processing Thai text.
- NLTK: The Natural Language Toolkit, adapted for Thai through PyThaiNLP.

### Data Source

The analysis utilizes a reference dataset that exercises both meaning and syntactic criteria based on linguistic knowledge and the Royal Thai dictionary.

### Key Findings

- Word Tokenization: 
  - Deepcut achieves an accuracy score of 94%, outperforming the NewMM engine which achieves 87%.
- Sentence Tokenization: 
  - The accuracy score for sentence tokenization is very low at 1%, indicating a need for more robust linguistic rules.
- Spellcheck: 
  - The overall character error rate for slang terms is noted at 0.59, with a system error rate of 0.61. Limitations stem from a small corpus and emerging new slangs.
- Named Entity Recognition (NER): 
  - Incomplete tagging may arise from incorrect tokenization and limited NER training corpus.

## Results Summary

- The NewMM engine performs a certain percentage faster than Deepcut.
- Tokenization is the most effective module in PyThaiNLP, delivering satisfactory accuracy scores and rapid tokenizing speeds.
- Other modules, however, demonstrate subpar performance, indicating the need for further development and an enhanced training dataset.

## Source Code

The source code used for this project is available [here](https://github.com/PyThaiNLP/pythainlp).

## Conclusion

This project highlights the effectiveness of the PyThaiNLP library for word tokenization while demonstrating room for improvement in other NLP tasks. Future work will focus on developing better training datasets and enhancing algorithms for improved performance.
