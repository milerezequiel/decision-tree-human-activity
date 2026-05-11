# Decision Tree - Human Activity Recognition

This project uses a human activity recognition dataset based on smartphone sensor data.  
The original dataset was already divided into training and test sets.

## Objective

The objective was to train a decision tree model to classify human activities using selected variables from the dataset.

Only three explanatory variables were used:

- `tBodyAcc-mean()-X`
- `tBodyAcc-mean()-Y`
- `tBodyAcc-mean()-Z`

## Steps

1. Loaded the dataset files.
2. Organized the training and test datasets.
3. Selected the three required variables.
4. Trained a decision tree with `min_samples_leaf=20`.
5. Calculated the `ccp_alpha` values for tree pruning.
6. Trained multiple trees using different `ccp_alpha` values.
7. Evaluated accuracy on the training and test sets.
8. Selected the best tree based on test accuracy.

## Libraries Used

- pandas
- numpy
- matplotlib
- scikit-learn

## Result

The best accuracy obtained using only the three selected variables was approximately **44.86%** on the test set.

This result shows that the model has limited classification performance when using only three variables. However, the project was useful to practice decision trees, pruning with `ccp_alpha`, and performance comparison between training and test data.

## Dataset

The dataset used was:

**Human Activity Recognition Using Smartphones Dataset**  
Available at the UCI Machine Learning Repository.

## Author

Miler Ezequiel dos Santos
