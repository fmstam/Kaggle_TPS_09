# Kaggle_TPS_09

It turns out that, this competition's main focus was how to handel the missing values, and the best solution was to add the number of missing.
I have tried different ways of imputation based on the distribution: from simple imputing like mean and median to end-tail. In fact, the difference between imputing the missing values and no-imputation was not significant because modern GBDT models are aware of the sparsity of the data.

Parts of my solution of this competition include, diversify the base-models therefore, I have used:
- neural network models
- different seeds 
- stacking with mixture of base models 
- features encoding,

blending was also effective in this competition due to the size of the data.
The plan was to study the local cross-validation and the LB scores and try to make sure there is a correlation between them to avoid overfitting. 