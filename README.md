# POS-Tagger-NLTK

This project implements a part-of-speech (POS) tagger using the Natural Language Toolkit (NLTK). The tagger is built by combining unigram and bigram models, with a fallback default tagger to handle unseen words. The model is trained on the Treebank corpus and is designed to tag words in a sentence according to their syntactic roles.

## Features

- Uses **NLTK** for POS tagging and tokenization.
- Combines **UnigramTagger** and **BigramTagger** for more accurate predictions.
- Implements a **DefaultTagger** to handle unseen words.
- Evaluates performance with accuracy, achieving around 88.31% on the test set.
- Easy to extend or replace with more complex models or datasets.

## Installation

To get started, make sure you have **Python** and **NLTK** installed. Follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/ahmdmohamedd/POS-Tagger-NLTK.git
   cd POS-Tagger-NLTK
   ```

2. Install the required dependencies:
   ```bash
   pip install nltk
   ```

3. Download necessary NLTK datasets:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('averaged_perceptron_tagger')
   nltk.download('treebank')
   ```

4. Run the Jupyter notebook:
   ```bash
   jupyter notebook POS_Tagging_with_NLTK.ipynb
   ```

## Usage

In the notebook, a test sentence is passed through the POS tagger, and the words are tagged with their corresponding part of speech (e.g., `NN` for noun, `VBZ` for verb). You can modify the test sentence to try different examples.

## Accuracy

The accuracy of the tagger on the test set is **88.31%**, which demonstrates good performance for basic POS tagging tasks. However, the accuracy may vary with more complex or domain-specific texts.

## Contributions

Feel free to fork the repository, improve the tagger, or suggest changes. Pull requests are welcome!
