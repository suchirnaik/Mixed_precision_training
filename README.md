# Mixed Precision Training for Sentiment Analysis with BERT

This project demonstrates **Mixed Precision Training** using the BERT model for sentiment analysis on the IMDb dataset. We compare three different training methods:

1. **No Mixed Precision** (FP32)
2. **Automatic Mixed Precision (AMP)**
3. **Manual Mixed Precision**

## Project Overview

Mixed precision training allows us to use both FP32 (full precision) and FP16 (half precision) in order to boost training speed while maintaining model accuracy. This project showcases how mixed precision training can be applied to a real-world NLP task using the BERT model.

The project is split into the following sections:

- **Data Preparation**: The IMDb dataset is loaded, tokenized, and prepared for training.
- **Training Methods**: The model is trained using no mixed precision, automatic mixed precision, and manual mixed precision to compare performance and results.
- **Evaluation**: After training, the model's performance is evaluated using accuracy, precision, recall, F1-score, and a confusion matrix.
  
## Results

### No Mixed Precision
- Training Time: ~640 seconds
- Evaluation Time: ~22.79 seconds
- Accuracy: 86.80%
- Precision: 90.12%
- Recall: 82.27%
- F1-Score: 86.02%

### Automatic Mixed Precision (AMP)
- Training Time: ~297.29 seconds
- Evaluation Time: ~15.38 seconds
- Accuracy: 86.10%
- Precision: 89.26%
- Recall: 81.66%
- F1-Score: 85.29%

### Manual Mixed Precision
- Training Time: ~643.49 seconds
- Evaluation Time: ~22.52 seconds
- Accuracy: 86.55%
- Precision: 85.17%
- Recall: 88.02%
- F1-Score: 86.57%

