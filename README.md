# Phishing-Email-Classifier-With-Adversarial-Machine-Learning
A study on the semantic differences between emails of different time eras through the use of machine learning, detecting these semantic differences to identify phishing emails, and then finally how adversarial inputs affects these models.


Within this ZIP file there are 3 subfolders, 5 CSVs, and 12 Google Colabs.

How to run project.


1) Establish Datasets, notebook is the first to be run. This notebook will clean and preprocess all the .csv files (which are in the Datasets folder) to create the 3 time-series based datasets all models will use.
	-Within this notebook, there should be a PROJECT_ROOT variable. Changed that accordingly, and all future notebooks should run interconnectedly.

2) Comparing Datasets, this notebook was only used to create the word embedding comparison of each dataset.

3) Authentic Data Ensemble Folder (Real Data), this folder contains the notebooks for the Base/Deep pipelines of all authentic data. Make sure to run the Base Pipelines BEFORE the Deep Pipelines to ensure they use the same train/test split. Then, after model is trained it's parameters & basic evaluation metrics will be uploaded within the Datasets/Models folder

4) Synthetic Data Ensemble Folder (Fake Data), this folder contains the pipelines for the Synthetic Data. Same as the previous ensemble folder.


5) Evaluation & Comparison (With Timeout Insurance), this notebook is where we run TextFooler onto all models and display all metrics.
