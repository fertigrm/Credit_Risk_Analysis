# Credit_Risk_Analysis
## Overview of Analysis
In this analysis, we deployed Python and its powerful libraries to build and test machine learning models to predict potential credit risk.
## Resources Used
- Python, Anaconda, Jupyter Notebook
## Findings
**BalancedRandomForestClassifier**
![Brfc_acc](https://user-images.githubusercontent.com/102084269/185446690-7b99cd24-d9db-4732-b33d-f217691d129d.PNG)
![brfc_cm](https://user-images.githubusercontent.com/102084269/185446702-a37992c9-e30f-4aee-a067-32d648d303ba.PNG)
![brfc_unbalanced](https://user-images.githubusercontent.com/102084269/185446708-435bf9db-e276-4998-9857-d60313a819b6.PNG)
With these images from our model we can see an accuracy score of roughly 79%
We can see the high risk precision is very low at 4% with an f1 score of 7%
The low risk precision however is practically 100%

**EasyEnsembleClassifier**
![easy_ensemble_acc](https://user-images.githubusercontent.com/102084269/185447295-05e3d746-078f-41dd-af67-2137eff772ab.PNG)
![EE_cm](https://user-images.githubusercontent.com/102084269/185447299-51b4c4bc-1714-42b7-84cc-df2b2489565b.PNG)
![EE_imbalanced](https://user-images.githubusercontent.com/102084269/185447305-094f4e1e-ec6b-48d7-959e-367b09d9eca4.PNG)
These images show the EasyEnsemble model was able to have an accuracy score of 93%
The high risk precision is low at around 7% with the f1 14%
The low risk precision is 99%

**RandomOverSampler**
![RandomOversamplerAccScore](https://user-images.githubusercontent.com/102084269/185447759-19f7ca10-180b-4326-b60d-02950139dfd5.PNG)
![ROversampler_cm](https://user-images.githubusercontent.com/102084269/185447776-aeb018e9-82a1-4111-afea-5ef953180e33.PNG)
![ROversampler_imbalanced_creport](https://user-images.githubusercontent.com/102084269/185447781-0866a684-b024-4fcd-8b6f-428ff441c8ad.PNG)
The RandomOverSampler model had an accuracy score of only 63%
The high risk precision is only 1% with an f1 score of 2%
The low risk precision is almost 100%

**SMOTE**
![SMOTE_acc](https://user-images.githubusercontent.com/102084269/185448099-9bfbd5e9-faba-47eb-889e-31835ecbc76a.PNG)
![SMOTE_cm](https://user-images.githubusercontent.com/102084269/185448116-b62079bf-12d3-4c69-b773-9aba8485b10e.PNG)
![SMOTE_imbalanced](https://user-images.githubusercontent.com/102084269/185448124-4bb300fe-12de-4eb0-8972-e00f6dd32010.PNG)
The SMOTE model had an accuracy score of around 65%
The high risk precision is 1% with an f1 score of 2%
The low risk precision is nearly 100%

**SMOTEEN**
![SMOTEEN_acc](https://user-images.githubusercontent.com/102084269/185448400-e85d1693-3adf-4aef-bb9e-ff3cbcaf3cbe.PNG)
![SMOTEEN_cm](https://user-images.githubusercontent.com/102084269/185448432-0549c045-2164-421c-b869-e168e2c5f523.PNG)
![SMOTEEN_unbalanced](https://user-images.githubusercontent.com/102084269/185448456-ab0fd389-bb4f-452b-8fdd-e7a99b614755.PNG)
The SMOTEEN model had an accuracy score of around 62%
The high risk precision was 1% with an f1 of only 2%
The low risk precision was 100%

**ClusterCentroids**
![Undersampled_acc](https://user-images.githubusercontent.com/102084269/185448814-85ebe437-b602-4f11-a148-7cdb505fce96.PNG)
![Undersampled_cm](https://user-images.githubusercontent.com/102084269/185448836-6fa76821-7fb1-443a-89a0-29935ccd9fa1.PNG)
![undersampled_unbalanced](https://user-images.githubusercontent.com/102084269/185448850-883f65eb-ba7e-43b7-b3d2-bd5100ff60a5.PNG)
The ClusterCentroids model had an accuracy score of around 53%
The high risk precision was 1% with an f1 of 1%
The low risk precision was 100%

## Summary of Analysis
All the models show a low precision in being able to determine wether or not the credit risk is high.
Due to this, I am not confident in recommending any of these models to be used.

