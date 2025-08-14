# SUMMARY

- Dataset: 100,000 ratings from 943 users for 1682 movies.
- User-item matrix created from ratings data.
- User similarity and item similarity computed using cosine similarity.
- User-based and item-based collaborative filtering implemented.
- Evaluation (Precision@10) yielded 0.0000 for both methods.
- SVD with `surprise` library failed due to numpy compatibility issues.

## Conclusion
- Very low precision suggests issues possibly due to data sparsity, similarity metric choice, or recommendation aggregation.
- Further investigation and alternative approaches recommended.
