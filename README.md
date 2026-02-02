Модель предсказывает, является клиент плохим или хорошим для оформленяи кредитной карты. 

https://www.kaggle.com/datasets/rikdifos/credit-card-approval-prediction
Task: Build a machine learning model to predict if an applicant is 'good' or 'bad' client, different from other tasks, the definition of 'good' or 'bad' is not given. You should use some techique, such as vintage analysis to construct you label. Also, unbalance data problem is a big problem in this task.

Тип задачи: Бинарная классификация

Метрика (ROC-AUC / F1)


По итогу выполненной работы, были обученны 2 модели, проведены One-Hot Coding, масштабирование.
1)LogistigRegression. Были получены следующие метрики:
Log loss train: 0.25099634208355737
Log loss test: 0.6716942477346365

precision    recall  f1-score   support

           0       1.00      0.98      0.99     18570
           1       0.88      1.00      0.93      2787

    accuracy                           0.98     21357
   macro avg       0.94      0.99      0.96     21357
weighted avg       0.98      0.98      0.98     21357

ROC-AUC : 0.9888263533727154
PR-AUC : 0.8749448822776797

2)LogisticRegressionCV(ElasticNet). Были получены следующие метрики:

Log-loss train: 0.24376301810420417
Log-loss test: 0.2042085527032439

precision    recall  f1-score   support

           0       1.00      1.00      1.00     18570
           1       0.98      0.97      0.98      2787

    accuracy                           0.99     21357
   macro avg       0.99      0.99      0.99     21357
weighted avg       0.99      0.99      0.99     21357

ROC-AUC : 0.9859160317954407
PR-AUC : 0.9602328805296247
