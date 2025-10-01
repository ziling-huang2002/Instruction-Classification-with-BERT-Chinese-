# Instruction Classification with BERT (Chinese)
This repository is part of my coursework for the Kaggle HW1 Instruction Classifier competition. The goal is to classify Chinese instructions into three operation types: replace, insert, and delete. I fine-tuned a BERT-based Chinese pretrained model and incorporated several architectural enhancements to improve classification performance.

## How to Run

1. **Clone the repository**  
```bash
   git clone https://github.com/ziling-huang2002/Instruction Classification with BERT (Chinese).git
   cd Instruction Classification with BERT (Chinese)
```

2. **Run**
  <br>Open [`main.ipynb`](main.ipynb) using Jupyter Notebook or VSCode and execute all cells in order.

## Result
| Class         | Precision | Recall | F1-Score | Support |
|---------------|----------|-------|----------|--------|
| 0             | 0.943    | 0.971 | 0.957    | 206    |
| 1             | 0.985    | 0.929 | 0.956    | 211    |
| 2             | 0.945    | 0.986 | 0.965    | 140    |
| **Accuracy**  |          |       | 0.959    | 557    |
| **Macro Avg** | 0.958    | 0.962 | 0.959    | 557    |
| **Weighted Avg** | 0.960 | 0.959 | 0.959    | 557    |

![Loss and Accuracy Curve](images/loss_accuracy_curve.png)
![Confusion Matrix](images/bert_confusion_matrix.png)
