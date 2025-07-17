# 🔤 Autocorrect NLP in Python

This project is a simple but effective **autocorrect tool** built using Natural Language Processing (NLP) with Python and NLTK. It mimics how common autocorrect systems work by generating candidate corrections and selecting the most probable word based on word frequency.

---

## 🚀 Features

- Tokenizes and normalizes text data
- Generates suggestions using common edit operations:
  - Letter deletion
  - Letter swapping
  - Letter replacement
  - Letter insertion
- Supports Level 1 and Level 2 corrections (single and double edit distance)
- Frequency-based word probability scoring
- CLI for interactive autocorrection

---

## 📁 Project Structure

autocorrect-nlp/
│
├── autocorrect.ipynb # Jupyter Notebook version (demo + explanation)
├── final.txt # Text dataset (used to build vocabulary)
├── README.md # Project documentation
└── requirements.txt # Python dependencies


---

## 🛠️ Setup Instructions

1. Clone the repository:

```bash
git clone https://github.com/iamsairamnagarajan/autocorrect-nlp.git
cd autocorrect-nlp
Install dependencies:

pip install -r requirements.txt

Make sure final.txt is in the root directory (this is your corpus for vocabulary)

How It Works
1) Preprocessing: Cleans and tokenizes the input dataset.

2) Frequency Calculation: Builds a dictionary of word frequencies from the corpus.

3) Candidate Generation: Applies edits (delete, swap, replace, insert) to produce potential corrections.

4) Probability Scoring: Calculates word probabilities based on frequency.
--

Example
Enter a word for autocorrection: wrd

Top suggestions:
1. word
2. ward
3. weird


Future Improvements
1)Add n-gram or contextual suggestions

2)Integrate with Transformer-based models (like BERT or RoBERTa)

3)Create a Streamlit or Flask-based web app UI

4)Deploy as an API or microservice
Suggestion Ranking: Suggests top-N most probable corrections.
