# Sentiment Analysis on SnapFood Comments Using Fine-Tuned AIpart_Tooka and Hazm

This project focuses on sentiment analysis of Persian (Farsi) user comments from the SnapFood platform. We fine-tuned the Persian pre-trained `[https://huggingface.co/PartAI/Tooka-SBERT]` model using custom labeled data. The input text is first preprocessed using the **Hazm** library to normalize and tokenize Persian language structure before feeding it to the model.
---

## 📊 Project Overview

- **Goal**: Automatically detect the sentiment (positive or negative) in Persian text reviews from the SnapFood app.
- **Model Used**: a sentence-transformers model trained (PartAI/TookaBERT-Base)
- **Preprocessing**: Normalization, tokenization, and stopword removal using [`hazm`](https://github.com/sobhe/hazm).
- **Language**: Persian (Farsi)
- **Frameworks**: PyTorch, Hugging Face Transformers, Datasets, Hazm
- **Final Accuracy**: **88%**

some examples

| خیلی خوشمزه بود و سریع رسید      | Positive   |
| کیفیت غذا افتضاح بود و دیر رسید  | Negative   |
| پیک مؤدب بود، دوباره سفارش می‌دم | Positive   |
| غذا سوخته بود، تجربه‌ی بدی بود   | Negative   |
