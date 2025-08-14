# SUMMARY

- Dataset: 10,000 entries, 55 integer columns, no missing values.
- Target variable for XGBoost adjusted to be zero-based.
- Initial results (before tuning):
  - Random Forest: Accuracy = 0.7970
  - XGBoost: Accuracy = 0.7970, slightly higher precision and F1 than RF.
- Feature importance analysis done on Random Forest.
- Hyperparameter tuning with `GridSearchCV` improved Random Forest accuracy to 0.8080.

## Best Parameters
```python
{'criterion': 'entropy', 'max_depth': None, 'min_samples_leaf': 1, 'min_samples_split': 2, 'n_estimators': 200}
```

## Conclusion
- Tuned Random Forest outperformed both the original RF and XGBoost across all metrics.
- Further optimization could improve results.
