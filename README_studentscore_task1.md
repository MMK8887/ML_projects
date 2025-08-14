# SUMMARY

- The dataset initially contained missing values in the 'Teacher_Quality', 'Parental_Education_Level', and 'Distance_from_Home' columns, which were handled by dropping the corresponding rows.
- The 'Hours_Studied' and 'Exam_Score' columns had no missing values and were of the appropriate data type.
- A scatter plot revealed a generally positive linear relationship between 'Hours_Studied' and 'Exam_Score'.
- A linear regression model trained on 'Hours_Studied' achieved:
  - Mean Squared Error (MSE): 12.35
  - R-squared (R2): 0.21
- A polynomial regression model with degree 2 yielded the same metrics as the simple linear model, indicating no benefit from the quadratic term.
- Including additional features ('Sleep_Hours', 'Extracurricular_Activities', and 'Parental_Involvement') improved results slightly:
  - MSE: 11.80
  - R2: 0.24

## Conclusion
- 'Hours_Studied' correlates with 'Exam_Score' but explains only 21% of the variance.
- Other factors significantly influence exam performance.