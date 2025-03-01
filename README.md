# Sentiment Analysis using BERT Transformers

## Overview
This project implements sentiment analysis using BERT (Bidirectional Encoder Representations from Transformers). The model classifies text reviews into three sentiment categories: Positive, Neutral, and Negative.

## Dataset
- The dataset used for this project contains customer reviews with ratings.
- The ratings are mapped to sentiment labels:
  - **0**: Negative (ratings ≤ 2)
  - **1**: Neutral (rating = 3)
  - **2**: Positive (ratings ≥ 4)

## Dependencies
Ensure you have the following dependencies installed:

```bash
pip install transformers torch pandas numpy seaborn scikit-learn matplotlib
```

## Steps
1. **Load Dataset:** The dataset (CSV format) is loaded into a Pandas DataFrame.
2. **Preprocessing:**
   - Convert ratings into sentiment labels.
   - Clean and tokenize text.
3. **BERT Tokenization:**
   - Use pre-trained BERT tokenizer.
   - Add special tokens like `[CLS]` and `[SEP]`.
4. **Model Training:**
   - Fine-tune BERT for sentiment classification.
   - Use a transformer-based classifier.
5. **Evaluation:**
   - Calculate accuracy, precision, recall, and F1-score.
   - Visualize results.

## Usage
Run the notebook or script to train and test the model:

```python
python train.py  # If using a script
```

Alternatively, execute the Jupyter Notebook for interactive execution.

## Results
- The model achieves high accuracy in sentiment classification.
- Predictions align well with human-labeled sentiments.

## Future Enhancements
- Experiment with different transformer architectures (e.g., DistilBERT, RoBERTa).
- Use larger datasets for better generalization.
- Deploy the model as an API for real-time sentiment analysis.

## Authors
- Hemanth
- 354he.35@gmail.com

