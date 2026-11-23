# Tree-Based Models: Random Forests

## Objective

I compared tree-based and linear regression models to predict California housing prices and examined how random forests improve predictive performance and measure feature importance.

## Methodology

- I fitted a single decision tree, OLS, Ridge regression, and a random forest using the California Housing dataset.
- I compared training and test performance using RMSE and R² to identify overfitting.
- I compared mean decrease in impurity (MDI) and permutation importance to evaluate the importance of each feature.
- I tuned the random forest's maximum depth and maximum features using cross-validation.
- I wrote my own AI prompt to generate a feature-importance chart and refined it over 2 rounds.
- I checked the AI-generated results against my original calculations and tested the function on a different model and dataset subset.

## Key Findings

The single decision tree achieved a test R² of 0.6228, while Ridge achieved 0.5758 and the random forest achieved 0.8046. I found that the single tree overfit the training data, while the random forest generalized better to unseen data.

Latitude had an MDI importance of 0.0890 but a permutation importance of 0.4427. This showed me how different methods of measuring feature importance can produce different results.

After tuning the random forest through cross-validation, its test R² improved to 0.8094.

My initial AI-generated function returned the correct feature rankings but slightly different importance values. After specifying the number of repeats and random seed in round 2, every numerical result matched exactly. This showed me the importance of writing precise prompts and independently verifying AI-generated results.
