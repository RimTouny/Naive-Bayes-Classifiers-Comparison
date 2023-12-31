# **Naive-Bayes-Classifiers-Comparison**
Explored alternatives for improved performance in ML course, uOttawa 2023.
This repository contains Python code implementing a [Spambase Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/spambase/spambase.data) analysis comparing Naïve Bayes classifiers. Evaluated accuracy, confusion matrices on different splits in a Spame dataset as part of a Machine Learning course project at my study in the University of Ottawa in 2023.

- Required libraries: scikit-learn, pandas, matplotlib.
- Execute cells in a Jupyter Notebook environment.

## Binary-class classification problem
Task is to classify the email dataset into two classes: Spam / Not Spam.

### Independent Variables:
   +	57 Features related to word frequencies, character frequencies, and capital run lengths.
### Target variable:
   +	'Target' indicating the classification into two classes.


## **Key Tasks Undertaken**

1. **Dataset Splitting:**
   - Divided the dataset into 80% training and 20% test samples, preserving the split for later analysis.

2. **Classifier Evaluation (80/20 Split):**
   - Computed confusion matrices and accuracy scores for Gaussian and Multinomial Naïve Bayes classifiers on test data.
     ![merge_from_ofoct](https://github.com/RimTouny/Naive-Bayes-Classifiers-Comparison/assets/48333870/21dec124-f8d2-4abf-a10f-984fbcbadb86)
     ![image](https://github.com/RimTouny/Naive-Bayes-Classifiers-Comparison/assets/48333870/e6e7a4e3-51f5-4959-8bab-c01dfa21ceef)

     - Identified that both classifiers didn't predict any spam instances due to unbalanced test data.
     


3. **Further Evaluation:**
   - Employed train-test split function, noting dataset shuffling to avoid zero instances of 'spam' in test data.
     ![merge_from_ofoct](https://github.com/RimTouny/Naive-Bayes-Classifiers-Comparison/assets/48333870/8c3296f0-ef3a-474d-bc68-c1879860d84c)
    ![image](https://github.com/RimTouny/Naive-Bayes-Classifiers-Comparison/assets/48333870/bad81b8a-aa64-4b2b-b5fc-092daab9bfd9)
![image](https://github.com/RimTouny/Naive-Bayes-Classifiers-Comparison/assets/48333870/ae1cd56a-ae40-4e58-90e4-13039b0282b1)




4. **Alternate Classifier Assessment:**
   - Explored Bernoulli and Complement Naïve Bayes classifiers, comparing their performance metrics with Gaussian and Multinomial models.
     ![image](https://github.com/RimTouny/Naive-Bayes-Classifiers-Comparison/assets/48333870/20f4a49d-d649-4b3f-a5e7-efa02f8b592a)


5. **Subset Evaluation:**
   - Analyzed four subsets' accuracies, revealing varied performances due to biased training on specific class labels.

6. **Visualization:**
   - Presented subset accuracies via a bar chart, highlighting classifier performance variations.
     ![image](https://github.com/RimTouny/Naive-Bayes-Classifiers-Comparison/assets/48333870/8f02fa0a-baa6-4bb3-8ed4-f40379b649c8)

