# Plagiarism Detection Using String Matching Algorithms

This project implements a plagiarism detection system by comparing two text documents using three classical string matching algorithms:

- **Knuth-Morris-Pratt (KMP)**
- **Boyer-Moore**
- **Rabin-Karp**

Each algorithm operates on preprocessed and stemmed versions of the documents to identify similar or overlapping sentences, providing both match counts and a plagiarism rate.

---

---

##  Algorithms Used

### 1. Knuth-Morris-Pratt (KMP)
- Efficient for substring search using prefix tables.
- Searches stemmed and normalized sentences from both documents.
- Used to detect partial or approximate sentence matches.

### 2. Boyer-Moore
- Skips unnecessary comparisons using a bad character heuristic.
- Fast for longer texts.
- Applied to exact matches on cleaned document strings.

### 3. Rabin-Karp
- Uses a rolling hash to detect possible matches quickly.
- Suitable for detecting multiple patterns in a larger body of text.
- Matches are confirmed with character-by-character comparison.

---

##  Preprocessing

Before applying the algorithms, the documents undergo:
- Sentence tokenization
- Stopword removal (basic list)
- Stemming using NLTK’s `PorterStemmer`
- Lowercasing and whitespace normalization

---


