
# Optional Machine-Learning Extension

## Objective

The model predicts whether a referral will be completed.

The target was defined as:

- 1 = completed referral
- 0 = not-completed referral

Referrals with blank or unknown outcomes were excluded from modelling.

## Validation approach

A time-based train/test split was used. The earlier 75% of referrals were used
for training, while the later 25% were used for testing.

This approach simulates using historical records to predict future referral
outcomes.

## Models evaluated

The following models were compared:

1. Majority-class baseline
2. Logistic regression
3. Random forest

The best model based on average precision was:

> **Random Forest**

## Test-period performance

| Metric | Result |
|---|---:|
| Accuracy | 0.595 |
| Precision | 0.755 |
| Recall | 0.702 |
| F1 score | 0.727 |
| ROC-AUC | 0.506 |
| Average precision | 0.798 |

## Operational use

The model produces a predicted non-completion risk for each referral.

The highest-risk referrals can be prioritized for:

- CHW follow-up
- Facility confirmation
- Supervisor review
- Transport or referral support
- Documentation reconciliation

## Limitations

This model should be treated as a prioritization tool rather than an automated
decision-maker.

The main limitations are:

- The dataset is synthetic.
- The referral sample is limited.
- Training and supervision records are not included.
- Model performance may change on future data.
- Predictions should be reviewed by program staff.
- The model may reproduce existing documentation or access inequalities.
