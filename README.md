# Tokenizer-on-English-and-Spanish
* [1 Introduction](#1-introduction)  
* [2 Getting Started](#2-getting-started)  
  * [2.1 Preparations](#21-preparations)  
  * [2.2 Install Packages](#22-install-packages)  
  * [2.3 Run Tokenizer](#23-run-n-gram)  

---

# **1. Introduction**

This project demonstrates building custom tokenizers using a WordPieace approach for mulitple langauges: English, Python code, and Spanish. The tokenizers are trained on small datasets and tested on sample text ot showcase performance

---

# **2 Getting Started**
This project is implemented in Jupyter Notebooks using Python 3.9+ and is compatible with macOS, Linux, and Windows.

## **2.1 Preparations**
(1) Clone the repository to your workspace

```shell
~ $ git clone https://github.com/ViolettGee/Tokenizer-on-English-Spanish-Python.git
```

## **2.2 Install Packages**
(2) Install the required dependecies:

```shell
~ $pip install tokenizers
```

## **2.3 Run Tokenizer**
The script should be run by runnning each of the nodes within the Jupyter Notebook file. The model is ready to run; however, if you would like to use your own data, you may exchange it wiht the data in the files. Keep in mind that the files in the "English" and "Spanish" folders should both be formatted as .txt file, and the files in the "Python" folder should be formated as .py files.

"tok.ipynb" The file creates a tokenizer's for and tokenizes each of the Languages: English, Python, and Spanish. Each language is loaded into a dataset from the files located in the respective folders. The text is then normalized to become strip white-space and make all text lower case. Then, the tokenizer is initialized with a pre-toknizer before training the tokenizer on its respective dataset. Once trained, each tokenizer is trained they are tested by encoding a new sample and printing the found tokens.

## **3. Results**
They python tokenizer performed the best having less unknowns, likely due to the repetitive nature of the language. The English and Spanish had more unknown tokens suggesting that more training data is needed for better coverage. Overall, the WordPiece approach provides meaningful subword tokenization across different languages and text types.
