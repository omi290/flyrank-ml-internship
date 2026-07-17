# Week 2 – Machine Learning Foundations

## My ML Task

### Problem

Prioritize website content pages for refresh based on historical search and engagement performance.

---

## Why Machine Learning?

A fixed rule such as "refresh every page with fewer than 100 clicks" cannot capture the relationships between multiple search and engagement signals.

A machine learning model can combine historical performance metrics to rank pages according to their likelihood of benefiting from a content refresh.

---

## ML Task Type

**Ranking / Scoring**

The goal is to rank pages by their predicted content opportunity rather than simply classifying them into fixed categories.

---

## Input Features

Examples of features include:

- GSC Impressions
- GSC Clicks
- Average Search Position
- GA4 Pageviews
- GA4 Sessions

Only information available before the prediction time is used.

---

## Prediction Target

A content opportunity score (or another future performance proxy defined later in the project).

---

## Success Metrics

Possible evaluation metrics include:

- NDCG
- Precision@K
- Recall@K

The final metric will depend on the modeling stage.

---

## Core Concepts Learned

### AI vs Machine Learning

Artificial Intelligence is the broader field of creating intelligent systems. Machine Learning is a subset of AI that learns patterns from data.

### Machine Learning vs Analytics

Analytics explains what has happened using historical data. Machine Learning predicts future outcomes or recommends actions.

### Machine Learning vs Rules

Rule-based systems rely on manually defined conditions.

Machine Learning discovers patterns automatically from data and can adapt better to complex relationships.

### Supervised vs Unsupervised Learning

- Supervised learning uses labeled data.
- Unsupervised learning discovers hidden patterns without labels.

### Generalization vs Overfitting

A useful model should generalize to unseen data instead of memorizing the training data.

---

## Conclusion

For my FlyRank capstone, a ranking/scoring machine learning approach is the most appropriate because the objective is to prioritize content pages for refresh using historical search and engagement signals while avoiding data leakage.
