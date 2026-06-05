# Bangla–Banglish Book Review Corpus (BBBRC)

A Fine-Grained Mixed-Script Dataset and Benchmark for Literary Sentiment Analysis

## Overview

The Bangla–Banglish Book Review Corpus (BBBRC) is a large-scale manually annotated dataset designed for fine-grained sentiment analysis of literary reviews written in both Bengali script (Bangla) and Romanized Bangla (Banglish).

The corpus contains 24,934 user-generated book reviews collected from online literary platforms and is annotated into four sentiment categories:

* Literary Appreciation
* Analytical Reflection
* Constructive Critique
* Strong Critique

The dataset addresses an important gap in Bangla NLP by providing a benchmark for mixed-script sentiment analysis and transliteration-aware language modeling.

---

## Dataset Statistics

| Dataset  | Reviews |
| -------- | ------- |
| Bangla   | 12,659  |
| Banglish | 12,275  |
| Combined | 24,934  |

### Label Distribution

| Label                 | Count  |
| --------------------- | ------ |
| Literary Appreciation | 17,850 |
| Analytical Reflection | 4,887  |
| Constructive Critique | 1,408  |
| Strong Critique       | 789    |

 

## Dataset Format

Each record contains:

| Column        | Description              |
| ------------- | ------------------------ |
| Review_ID     | Unique review identifier |
| Bangla_Text   | Bengali script review    |
| Banglish_Text | Romanized Bangla review  |
| Combined_Text | Unified review text      |
| Label         | Sentiment category       |

---

## Proposed Models

This repository includes implementations of:

### Baseline Models

* FastText + Logistic Regression
* FastText + Linear SVM
* DistilBERT Multilingual
* mBERT
* XLM-RoBERTa
* MuRIL

### Proposed Architectures

* TA-MuRIL (Transliteration-Aware MuRIL)
* TA-XLM-R (Transliteration-Aware XLM-RoBERTa)

The proposed architectures combine:

* Contextual transformer embeddings
* Character-level transliteration-aware representations
* Attention-based feature fusion
* Focal loss optimization

for robust mixed-script sentiment classification.

 

## Data Availability

The Bangla–Banglish Book Review Corpus (BBBRC), annotation guidelines, source code, and experimental resources are publicly available for research and educational purposes.

The dataset is archived through Zenodo and can be accessed using its DOI.

---

## Citation

If you use BBBRC in your research, please cite:

Pronay, R. H., & Spriha, N. J. (2026). *Bangla–Banglish Book Review Corpus (BBBRC): A Fine-Grained Mixed-Script Dataset for Literary Sentiment Analysis* [Data set]. Zenodo.

---

## License

This dataset is released for research and educational purposes under an open license.

Please cite the dataset when using it in academic publications.

---

## Contact

**Rafsan Hasan Pronoy**

Department of Computer Science and Engineering

Email: [rafsanhasanpronoy00@gmail.com](mailto:your-email@example.com)

GitHub: https://github.com/RafsanHasanPronoy
