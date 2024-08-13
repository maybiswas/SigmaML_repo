SigmaML Quiz 2 : Fashion MNIST Ablation Study
=============================================

Project Details
---------------

* Github Repository : https://github.com/maybiswas/SigmaML_repo

* Main Notebook : https://github.com/maybiswas/SigmaML_repo/blob/main/notebooks/FashionMNIST_ablation_study.ipynb

* Training data : https://www.tensorflow.org/api_docs/python/tf/keras/datasets/fashion_mnist
![Training_subset](https://github.com/user-attachments/assets/6fbde16a-266f-4cb4-a14d-d4e4048dfcf4)

* Problem Statement : To perform ablation study of sequential dense layers in a 10-label classification problem.

* Ablation Table - Performance Comparison : https://github.com/maybiswas/SigmaML_repo/blob/main/reports/FashionMNIST_ablation_study_table.csv

|Experiment No.|Experiment Directory|Experiment Title|Accuracy%|
|---|---|---|---|
|1|FashionMNIST_expt1|3 Sequential layers : 200 + ReLU, 50 + ReLU, 10 + Sigmoid|87.42|
|2|FashionMNIST_expt2|4 Sequential layers : 200 + ReLU, 100 + ReLU, 50 + ReLU, 10 + Sigmoid|87.56|
|3|FashionMNIST_expt3|5 Sequential layers : 500 + ReLU, 200 + ReLU, 100 + ReLU, 50 + ReLU, 10 + Sigmoid|88.61|
|4|FashionMNIST_expt4|7 Sequential layers : 500 + ReLU, 350 + ReLU, 200 + ReLU, 100 + ReLU, 50 + ReLU, 25 + ReLU, 10 + Sigmoid|87.91|
|5|FashionMNIST_expt5|10 Sequential layers : 1000 + ReLU, 800 + ReLU, 650 + ReLU, 500 + ReLU, 350 + ReLU, 200 + ReLU, 100 + ReLU, 50 + ReLU, 25 + ReLU, 10 + Sigmoid|88.18|
|6|FashionMNIST_expt6|2 Sequential layers : 10000 + ReLU, 10 + Sigmoid|88.29|
|7|FashionMNIST_expt7|2 Sequential layers : 500 + ReLU, 10 + Sigmoid|88.5|
|8|FashionMNIST_expt8|3 Sequential layers : 50 + ReLU, 30 + ReLU, 10 + Sigmoid|87.17|
|9|FashionMNIST_expt9|3 Sequential layers : 50 + ReLU, 30 + ReLU, 10 + Softmax|87.01|
|10|FashionMNIST_expt10|5 Sequential layers : 100 + ReLU, 50 + ReLU, 150 + ReLU, 50 + ReLU, 10 + Sigmoid|87.17|


* Sample Test data with Results with predicted labels [for one of the experiments (FashionMNIST_expt10)] : 
![Test_images](https://github.com/user-attachments/assets/0720a875-3e6e-4377-af1e-751a60909b42)

* Above test images / tensorboard / logs for each experiment can be found @ path - "SigmaML_repo/logs/FashionMNIST_expt1/"





Project Organization
--------------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
