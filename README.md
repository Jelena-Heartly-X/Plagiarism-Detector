# Plagiarism Detector

A GUI-based plagiarism detection tool built with **Python**, **Tkinter**, and **NLTK**. It compares input text against a folder of `.txt` files and highlights potential plagiarism using **n-gram similarity** and **longest common substring (LCS)**.

---

## Features

- Simple GUI using Tkinter  
- N-gram based plagiarism detection  
- Longest Common Substring comparison  
- Handles multiple `.txt` reference documents  
- Detailed scrollable plagiarism report  
- Saves submitted text with a timestamp

---

## How It Works

1. Tokenizes and lemmatizes the input using **NLTK**.
2. Generates **n-grams** for input and reference texts.
3. Inserts reference n-grams into a **Trie data structure**.
4. Computes similarity score by matching input n-grams in the Trie.
5. Detects **Longest Common Substring (LCS)** between matching texts.
6. Displays results in a GUI and saves the input.

---

## How to Run

### 1. Clone the repository:
```bash
git clone https://github.com/Jelena-Heartly-X/plagiarism-detector.git
cd plagiarism-detector
```

### 2. Install dependencies:
```bash
pip install nltk
```

### 3. Download NLTK resources (run once in Python)::
```bash
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```

### 4. Run the application:
```bash
python plagiarism_checker.py
```

## Requirements:

- Python 3.6 or above
- nltk
- tkinter (comes pre-installed with Python on most systems)
