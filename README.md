Comparative Evaluation of Classical Machine Learning Algorithms for Breast Cancer Classification

Project Overview

This project compares three classical machine learning algorithms for classifying malignant and benign cases using the Breast Cancer Wisconsin Diagnostic dataset.

The algorithms evaluated are
* Logistic Regression
* K-Nearest Neighbours (KNN)
* Random Forest

The experiment focuses on comparing model performance using accuracy, precision, recall, F1-score and confusion matrices.

Research Question

How do Logistic Regression, K-Nearest Neighbours and Random Forest compare in their ability to classify malignant and benign cases using the Breast Cancer Wisconsin Diagnostic dataset?

Dataset

The dataset was loaded using the load_breast_cancer() function from scikit-learn.

It contains:

* 569 observations
* 30 numerical input features
* 2 target classes

Target class mapping:

Label	    Class
0	        Malignant
1	        Benign

Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

Methodology

The experiment followed these steps:

1. Loaded and explored the dataset.
2. Separated input features and target labels.
3. Divided the data into training and testing sets using an 80/20 stratified split.
4. Applied feature standardisation to Logistic Regression and KNN using scikit-learn Pipelines.
5. Trained Logistic Regression, KNN and Random Forest.
6. Evaluated the models using classification metrics and confusion matrices.
7. Compared the results and examined classification errors.

The train-test split used random_state=42.

Experimental Results

The following results were obtained from the test set:

Metric	                 Logistic Regression	    KNN	            Random Forest
Accuracy	             98.25%	                    95.61%	        95.61%
Malignant Precision	     97.62%	                    95.12%	        95.12%
Malignant Recall	     97.62%	                    92.86%	        92.86%
Malignant F1-score	     97.62%	                    93.98%	        93.98%

Key Findings

* Logistic Regression achieved the highest accuracy on the selected test set.
* Logistic Regression also achieved the highest malignant-class recall.
* KNN and Random Forest produced identical confusion matrices in this experiment.
* The results demonstrate the value of evaluating classification models using multiple metrics rather than accuracy alone.

Limitations

* The models were evaluated using a single train-test split.
* Only three classical machine learning algorithms were compared.
* Extensive hyperparameter optimisation was not performed.
* No independent external dataset was used for validation.
* The experiment does not establish clinical reliability or medical suitability.

Conclusion

Logistic Regression demonstrated the strongest baseline performance among the three models on the selected test set.

Further evaluation using cross-validation, hyperparameter optimisation and independent datasets would be required to investigate the consistency and generalisability of the results.

This project is an educational machine learning experiment and is not intended for clinical diagnosis.

Reproducibility

To reproduce the experiment:

1. Clone this repository.
2. Install the dependencies listed in requirements.txt.
3. Open the Jupyter Notebook.
4. Run the notebook cells in order.

Author

Computer Engineering Graduate | Aspiring AI/ML Researcher

Interested in machine learning, data science and inclusive communication technology.