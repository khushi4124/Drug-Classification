# Drug-Classification
This Drug Classification project utilizes a Decision Tree Classifier to accurately predict prescribed medications based on patient health profiles. The implementation features a modular scikit-learn pipeline with a ColumnTransformer to handle various data types.

**Dataset Used**: https://www.kaggle.com/datasets/prathamtripathi/drug-classification

**My Solution**

I chose a Pipeline approach to keep the code clean and prevent data leakage.

The logic was to split the features based on their type. 

Since BP and Cholesterol have a natural order, I used ordinal encoding. 

For numeric values like the sodium-to-potassium ratio, I used scaling to ensure they are on the same level. 

I limited the tree size to 6 leaf nodes to make sure the model stays simple and easy to interpret.

**Results and Discussion**

The model achieved 100% accuracy on the test set.

**Performance Summary**

The classification report shows perfect precision and recall for all five drug classes (A, B, C, X, and Y).

  precision    recall  f1-score   support

           A       1.00      1.00      1.00         6
           B       1.00      1.00      1.00         3
           C       1.00      1.00      1.00         5
           X       1.00      1.00      1.00        11
           Y       1.00      1.00      1.00        15

    accuracy                           1.00        40
   macro avg       1.00      1.00      1.00        40
weighted avg       1.00      1.00      1.00        40

<img width="499" height="432" alt="image" src="https://github.com/user-attachments/assets/c499c6a6-e8c5-403c-b7e6-c156d20b4852" />



<img width="950" height="636" alt="image" src="https://github.com/user-attachments/assets/8155688a-0465-4442-9f5c-2d4806a751ca" />
