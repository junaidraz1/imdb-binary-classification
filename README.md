# IMDB Binary Sentiment Classification Dataset

This repository contains a preprocessing pipeline for transforming plain-text IMDB movie reviews into a machine-learning-ready dataset using the [`datasets`](https://huggingface.co/docs/datasets) library. The dataset is ideal for binary sentiment classification tasks.

---

## 📚 Dataset Description

The original data consists of two plain-text files, each containing one review per line:

- [Positive IMDB Reviews](http://dl.turkunlp.org/TKO_7095_2023/imdb-positives.txt)
- [Negative IMDB Reviews](http://dl.turkunlp.org/TKO_7095_2023/imdb-negatives.txt)

Each file represents a sentiment label (either `positive` or `negative`) and contains raw review texts.

For fulle dataset refer to the url below:
- [Imdb Binary Classification Dataset](https://drive.google.com/drive/folders/1sc2E4K9Nzaiow8oB3h7OK88mCO-eiga5?usp=sharing)

---

## 🛠️ Motive

Transform the above data into a structured dataset with the following specifications:

- Each example has:
  - `text`: The content of the movie review.
  - `label`: The sentiment label — either `positive` or `negative`.

- The dataset is split into:
  - `train` (80%)
  - `validation` (10%)
  - `test` (10%)

- All splits have a ~50/50 distribution of `positive` and `negative` reviews.

- The final output is a `DatasetDict` object with Hugging Face's `datasets` library, containing `Dataset` objects for each split.

---
