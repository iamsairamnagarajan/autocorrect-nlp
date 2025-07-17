
# 🔤 Autocorrect NLP in Python

A simple and effective **autocorrect tool** built using Natural Language Processing (NLP) techniques in Python. It simulates how modern autocorrect systems work by generating possible corrections and selecting the most probable word using frequency-based scoring.

---

## 🚀 Features

- Text normalization and tokenization
- Candidate suggestions via:
  - 🔡 Letter deletion
  - 🔁 Letter swapping
  - 🔤 Letter replacement
  - ➕ Letter insertion
- Single-edit (Level 1) and double-edit (Level 2) corrections
- Word frequency and probability-based ranking
- Interactive CLI for real-time autocorrection

---

## 📁 Project Structure

```
autocorrect-nlp/
│
├── autocorrect.ipynb         # Notebook with full implementation
├── final.txt                 # Corpus file used to generate vocabulary
├── requirements.txt          # Python package dependencies
└── README.md                 # Project documentation
```

---

## 🛠️ Setup Instructions

1. **Clone the repository**

```bash
git clone https://github.com/iamsairamnagarajan/autocorrect-nlp.git
cd autocorrect-nlp
```

2. **Install the dependencies**

```bash
pip install -r requirements.txt
```

3. **Ensure the dataset is available**

Place the `final.txt` file (corpus) in the root directory. This will be used to build the vocabulary and frequency dictionary.

---

## 🧠 How It Works

1. **Preprocessing**: Reads and cleans the corpus, then tokenizes it into lowercase words.
2. **Frequency Calculation**: Builds a dictionary that counts how often each word appears.
3. **Candidate Generation**: Creates possible correct spellings using edit operations (delete, insert, replace, swap).
4. **Level 2 Edits**: Applies edits again on Level 1 candidates to widen the correction range.
5. **Probability Scoring**: Calculates probabilities for each candidate based on frequency.
6. **Suggestion Ranking**: Returns the top-N suggestions with the highest probability.

---

## 💬 Example

```
Enter a word for autocorrection: wrd

Top suggestions:
1. word
2. ward
3. weird
```

---

## 🎯 Future Improvements

- [ ] Add n-gram-based contextual suggestions
- [ ] Integrate with Transformer-based models (e.g., BERT, RoBERTa)
- [ ] Build a user-friendly UI using **Streamlit** or **Flask**
- [ ] Deploy as a RESTful **API or microservice**

---

## 🤝 Contributing

Pull requests are welcome! If you find a bug or have suggestions, open an issue or fork and submit a PR. Let’s build something cool together. 😎

---



## 👤 Author

**Sairam Nagarajan**  
🔗 [GitHub](https://github.com/iamsairamnagarajan) | 🔗 [LinkedIn](https://linkedin.com/in/iamsairamnagarajan)

---

> 🚀 *“Smart tools make smart people even smarter. This project is one small step into intelligent text processing.”*
