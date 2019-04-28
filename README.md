# Google-Gendered-Pronoun-Resolution

**91th Place Solution** of GoogleAI Gendered Pronoun Resolution Competition in Kaggle.

[Gendered Pronoun Resolution](https://www.kaggle.com/c/gendered-pronoun-resolution)

![rank](img/rank.png)

## Two Model Strategy

- Model 1: Using BERT(768 uncased) as the embeddings, combine with different text features and distance features, feed into LightGBM model, using 5-fold to make predictions.

- Model 2: Adding head (3 layer linear network) on top of BERT 23 layers, use expand extractor extract distance information between pronoun and A&B.
