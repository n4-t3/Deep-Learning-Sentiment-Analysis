# Sentiment Analysis Deep Learning Model

## Overview
This repository contains a deep learning model for sentiment analysis using the IMDB review dataset from Kaggle. The model is a 3-layer feed-forward neural network that classifies text reviews as positive or negative.

## Model Architecture

The model consists of:
- **Embedding Layer**: Converts text into word embeddings (input_dim=5000, output_dim=128, input_length=200).
- **LSTM Layer**: 128 units with dropout and recurrent dropout to handle sequential dependencies in text.
- **Dense Layer**: A final sigmoid activation layer for binary sentiment classification (positive/negative).

---

## Dataset

The model is trained on the **IMDB movie review dataset** from Kaggle. You can access and download the dataset from the following link:

- [IMDB Dataset of 50K Movie Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

The dataset contains 50,000 movie reviews labeled as **positive** or **negative**.

---

## Testing Result

```python
new_reivew = "That movie was the best film this year"
sentiment = predict_sentiment(new_reivew)
print(f"The Sentiment of the review is: {sentiment}")
```
```
1/1 ━━━━━━━━━━━━━━━━━━━━ 0s 464ms/step
The Sentiment of the review is: positive
```

## License

This project is licensed under the BEER-WARE License - see the [LICENSE](LICENSE) file for details.

