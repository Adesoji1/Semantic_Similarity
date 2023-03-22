# Semantic_Similarity
Given a text and a reason, predict if text satisfies the reason. You can use the train file for any training and report metrics on evaluation file.
## **Dataset information**

- The CSV files have 3 columns
    - text
    - reason: a short description
    - label:
        - 0: text does not satisfy the reason
        - 1: text satisfies the reason
- The dataset has been cleaned to a certain extent. You can probe more.

**Note**: Small train dataset with only positive samples is intentional.

### Files

[https://drive.google.com/drive/folders/1HInfR5Sspv-k3rMPgJyXjXiJJEoCyOtY?usp=sharing](https://drive.google.com/drive/folders/1HInfR5Sspv-k3rMPgJyXjXiJJEoCyOtY?usp=sharing)

# **Solution Below**
The python scripts in this repository addresses the issues below. Run on Google colab, script can be found [here](https://colab.research.google.com/drive/1QStZaOSnlBo2ct3p9gPAmtW4ehPWqkdK?usp=sharing)

1. Required packages
2. Label class Imbalance
3. - Data insights:
      - Baseline approach (use only transformer models)
      - Training approach (use only transformer models)
      - Artificial neg generation techniques.
4. Metrics 
5. Ablation Study table (different tabular model architecture results comparison)
6. Fine-tuned the learning rate.
7. Used a learning rate scheduler.
8. Used a pre-trained model specifically designed for semantic similarity, such as sentence-transformers/bert-base-nli-mean-tokens.
9. Insufficient data from data insights analysis
