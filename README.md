# Parkinson-Disease-Detection-From-Voice-Recording

Dataset is taken from : https://archive.ics.uci.edu/ml/datasets/Parkinson+Speech+Dataset+with++Multiple+Types+of+Sound+Recordings

Problem Description:
Parkinson's disease is a progressive nervous system disorder that affects movement. The elderly people suffer from this disease. There are some symptoms of this disease such as Tremor, slowed movement (Bradykinesia), Rigid Muscles, Impaired posture and balance, Loss of automatic movements, speech changes or shaky speech, writing changes because of shaky hands. Among those symptoms, in this project we are using the changes in speech due to Parkinson Disease.

Dataset discussion:
In this dataset, we have 20 PD patient (6 female, 14 male) and 20 healthy individuals (10 female, 10 male). From all subjects, multiple types of sound recordings (26 voice samples including sustained vowels, numbers, words, and short sentences) are taken. A group of 26 linear and time frequency-based features are extracted from each voice sample. This dataset will be used to train the model. UPDRS ((Unified Parkinson’s Disease Rating Scale) score of each patient which is determined by expert physician is also available in this dataset. It can be used for regression purpose. However, we have to eliminate this column as we are dealing with classification.
After collecting the training dataset which consists of multiple types of sound recordings and performing our experiments, in line with the obtained findings we continued collecting an independent test set from PWP via the same physician’s examination process under the same conditions. During the collection of this dataset, 28 PD patients are asked to say only the sustained vowels 'a' and 'o' three times which makes a total of 168 recordings. The same 26 features are extracted from voice samples of this dataset. This dataset can be used to test the model that will be trained on the train dataset.

Training Data File:
The 26 features are distributed like below:
1: sustained vowel 2: sustained vowel 3: sustained vowel 4-13: numbers from 1 to 10 14-17: short sentences
18-26: words
Project goal
The goal of the project is to determine Parkinson Disease from those 168 recordings that had taken from 28 patient. We have to check how our trained model works. We have trained our

Test Data File:
The 26 features are distributed like below:
1-3: sustained vowel
4-6: sustained vowel
model with different Machine Learning Algorithms such as XGBoost, Logistic Regression, KNN, SVM, Naïve Bayes etc. We have to find out the best Algorithm that works on this dataset.

Solution:

After training the models, we tested the dataset that contained all of the Parkinson’s patient data. There were no healthy persons data in test set. So, It could not be checked. So, far the accuracy percentage we got for different algorithms is like below:
1. The Accuracy for XGBoost Algorithm = 68.45%
2. The Accuracy for Logistic Regression Algorithm = 91.67%
3. The Accuracy for Gaussian Naïve Bayes Algorithm = 85.12%
4. The Accuracy for KNN Algorithm = 83.93%
5. The Accuracy for SVM Algorithm = 62.50%
6. The Accuracy for Decision Tree Algorithm = 48.21%
Among the 6 algorithms we used for testing given dataset, we got the highest accuracy for the Logistic Regression whereas the lowest accuracy is for the Decision Tree.
