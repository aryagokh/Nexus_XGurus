# Nexus_XGurus - Final LeaderBoard Score - 0.9941675 Weighted F1 Score 
**Teammates :**
- Tirath Bhathawala
- Arya Gokhale
- Yash Prajapati

### File - FiguredOutCols_dropped_XGBoost.ipynb and 
First, we tried logically dropping some features which did not make much sense to us to keep them in training.
Then, converted categorical columns to numerical using LabelEncoding.
Then, we ran *Nearly All Classification Models* and found out that XGBoost was working the best.
The, we started *hyperparameter tuning the XGBoost* with *Optuna*
We saved some best params given by Optuna and parallely ran the same on test and train sets in another notebook.
Then, doing some more feature engineering we also did some research regarding the columns in the train sets.
We also ran the same Optuna for CatBoost and were training and predicting parallely.

### File - Advanced_FE_with_XGBandCAT
Then, we started completely fresh and ran some hyperparameters found earlier on all the columns.
Then, we did what improved our score the most **FEATURE ENGINEERING**
We ran **CORRELATION MATRIX** and **PLOT FEATURE IMPORTANCE** functions to get top related features.
Then, we dropped columns which had importance less than 2 %
Then, ran the same Hyperparameters of CatBoost on the dropped columns and got that 99% mark.

### File - StackingSubmission all versions (XGurus_main.ipynb here)
We then focused on stacking models as it helps it to generalize properly (used StackingClassifier)
Then, we ran some of those models and found the best one in that which gave us the score of 0.9939 (on public LB)
Then, similarly ran some of more models and feature engineering but didn't make much out of it.
