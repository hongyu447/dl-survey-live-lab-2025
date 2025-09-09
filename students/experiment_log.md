# Experiment Log (Your Name)

For each experiment you run this semester:
1. Copy the template block below.
2. Fill it in.
3. Add it to the bottom of this file.

---

## Experiment 01_baseline_random_forest

### Run #: 1
### Date:
### Goal / Question:
testing how num_estimators affects the classifier
### Setup: rf
rf2 = RandomForestClassifier(
    n_estimators=50,   # try 50 / 100 / 200
    max_depth=None,     # try 10 / 20 / None
    min_samples_split=2,  # try 2 / 5
    random_state=42
)
### Results:
              precision    recall  f1-score   support

       <=50K       0.88      0.92      0.90      7431
        >50K       0.71      0.61      0.66      2338

    accuracy                           0.85      9769
   macro avg       0.80      0.77      0.78      9769
weighted avg       0.84      0.85      0.84      9769

### Reflection:
(What worked? What didn’t? What would you try next?)

### Run #: 2
### Date:
### Goal / Question:
testing how num_estimators affects the classifier
### Setup: rf
rf2 = RandomForestClassifier(
    n_estimators=100,   # try 50 / 100 / 200
    max_depth=None,     # try 10 / 20 / None
    min_samples_split=2,  # try 2 / 5
    random_state=42
)
### Results:
             precision    recall  f1-score   support

       <=50K       0.88      0.92      0.90      7431
        >50K       0.72      0.61      0.66      2338

    accuracy                           0.85      9769
   macro avg       0.80      0.77      0.78      9769
weighted avg       0.84      0.85      0.85      9769

### Reflection:
(What worked? What didn’t? What would you try next?)

### Run #: 3
### Date:
### Goal / Question:
testing how num_estimators affects the classifier
### Setup: rf
rf2 = RandomForestClassifier(
    n_estimators=200,   # try 50 / 100 / 200
    max_depth=None,     # try 10 / 20 / None
    min_samples_split=2,  # try 2 / 5
    random_state=42
)
### Results:
              precision    recall  f1-score   support

       <=50K       0.88      0.93      0.90      7431
        >50K       0.72      0.61      0.66      2338

    accuracy                           0.85      9769
   macro avg       0.80      0.77      0.78      9769
weighted avg       0.84      0.85      0.85      9769

### Reflection:
Mininal changes

# Example Experiment Log — Taiwo 

## Run 1 — 2025-09-04
- **Goal / Question**: What happens if I change `n_estimators` from 100 to 200?
- **Setup**: Baseline Random Forest, train/test split = 80/20
- **Results**: Accuracy = 0.84, Precision = 0.72, Recall = 0.66
- **Reflection**: Increasing estimators gave a small accuracy bump. Took longer to train. Worth it? Maybe.

---

## Run 2 — 2025-09-06
- **Goal / Question**: Compare Random Forest vs Logistic Regression
- **Setup**: Same preprocessing as before
- **Results**: RF Acc = 0.85, LogReg Acc = 0.79
- **Reflection**: LogReg underfit the data. Nice reminder that not all models capture interactions.
