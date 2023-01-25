# Flash-Cards: A Question Generation Model

Flash-Cards is a Question Generation model that fine-tunes the T5 model using the Harvesting QA and SQuAD-v2 datasets. The goal of this model is to generate question based on given input text.

## Dataset
The Harvesting QA dataset was reduced to 128.6k for training and 1.6k for validation. SQuAD-v2 datasets size 130k for training and 11,8k for validation. This reduction was done to make the dataset more manageable for training the model.

## Hyperparameters
- Learning rate: 1e-4
- Number of training epochs: 3
- Optimizer: Adam Optimizer

## Evaluation Metrics
### SQuAD and Harvesting QA together
The model was evaluated using several metrics:

- BLEU score:
    - 1-gram: 0.63
    - 2-gram: 0.41
    - 3-gram: 0.31
    - 4-gram: 0.27
    - Cumulative BLEU score: 0.37
- METEOR score: 0.38
- ROUGE score:
    - ROUGE1: 0.42
    - ROUGE-L: 0.40
- F1 score:
    - Mean F1 score (ROUGE-1): 0.41
    - Mean recall (ROUGE-1): 0.42
    - Mean precision (ROUGE-1): 0.43
    - Mean F1 score (ROUGE-L): 0.40
    - Mean recall (ROUGE-L): 0.41
    - Mean precision (ROUGE-L): 0.41

### Harvesting QA
The model was evaluated using several metrics:

- BLEU score:
    - 1-gram: 0.63
    - 2-gram: 0.41
    - 3-gram: 0.31
    - 4-gram: 0.27
    - Cumulative BLEU score: 0.37
- METEOR score: 0.38
- ROUGE score:
    - ROUGE1: 0.42
    - ROUGE-L: 0.40
- F1 score:
    - Mean F1 score (ROUGE-1): 0.41
    - Mean recall (ROUGE-1): 0.42
    - Mean precision (ROUGE-1): 0.43
    - Mean F1 score (ROUGE-L): 0.40
    - Mean recall (ROUGE-L): 0.41
    - Mean precision (ROUGE-L): 0.41

## Conclusion

The Flash-Cards model performed well in generating questions based on the input text. The model achieved high scores on various evaluation metrics such as BLEU, METEOR, ROUGE and F1-score, indicating that the model is able to generate grammatically and semantically correct questions.
