# Heart-Failure-Prediction-using-AI
There are some factors that affects Death Event. 
# Methods:
1. Random Forest 
2. Logistic Regression 
3. SVM

# Heart-Failure-Prediction-using-Random-Forest
There are some factors that affects Death Event. This dataset contains person's information like age ,sex , blood pressure, smoke, diabetes, ejection fraction, creatinine phosphokinase, serum_creatinine, serum_sodium, time and we have to predict their DEATH EVENT.


# Data Source
[Heart Failure Prediction](https://www.kaggle.com/andrewmvd/heart-failure-clinical-data)


# Data Processing
This dataset is only 299 rows, which is not a very large dataset to train or
test on. So to be fair to both training and testing, I split the data into 50%
train and 50% test.
In addition, the data is originally uneven distributed respect to “DEATH
EVENT”. So, I rearranged the data sequence in random order to let both train
and test data have a close death rate.

# Prediction Target
There are some factors that affects Death Event. This dataset contains
person's information like age, sex, blood pressure, smoke, diabetes, ejection
fraction, creatinine phosphokinase, serum_creatinine, serum_sodium, time
and we have to predict their DEATH EVENT.


￼![image](https://user-images.githubusercontent.com/18226575/111269241-af92ec00-8671-11eb-8d49-799bbbe5b252.png)

# Background
Heart failure is a common event caused by cardiovascular diseases and this  dataset contains 12 features that can be used to predict mortality by heart  failure. 
People with cardiovascular disease or who are at high cardiovascular risk  need early detection and management where in a machine learning model  can be of great help. 

## テストデータに対する予測精度（Accuracy）： 
- Random Forest: 85% 
- Logistic Regression: 62％ 
- SVM: 70% 


1. Random Forest: 85%

|               | predicted 0   | predicted 1  |
| ------------- |:-------------:| -----:|
| actual 0      | 95            | 10     |
| actual 1      | 12            | 33    |

2. Logistic Regression: 62％ 

|               | predicted 0   | predicted 1  |
| ------------- |:-------------:| -----:|
| actual 0      | 92            | 13     |
| actual 1      | 17            | 28    |

3. SVM: 70%

|               | predicted 0   | predicted 1  |
| ------------- |:-------------:| -----:|
| actual 0      | 105            | 0     |
| actual 1      | 45            | 0    |


# Discussion
- SVM is giving only 0.7 which we might improve by using HyperParameter  tuning. However, it took too long that I did not include it in the report. - Among the three method, Logistic Regression has the worst  accuracy(62%) 
- I think the reason is the feature space is too large  
- Random Forest has a highest accuracy (85%). We might also improve it by  using HyperParameter tuning. 
- Random forests are inherently mutliclass whereas Support Vector Machines  need workarounds to treat multiple classes classification tasks.





