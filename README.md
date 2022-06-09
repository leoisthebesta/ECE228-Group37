# ECE228-Group37 Skin Lesion Classification
![dashboard_preview](/nb.jpeg)
---
## Table of Content
- [Introduction](#introduction)
- [Methodology and Results](#methodologyandresults)
- [Data Source](#datasource)
- [Code](#code)
- [File Structure](#filestructure)
- [Require Packages](#requirepackages)
- [Contributors](#contributors)
- [Citation](#citation)


<a name="introduction"></a>
## Introduction
There are many types of the skin lesion. Some of the them are not fatal and can be cured with appropriate treatment. However, some of them are actually cancer and they are fatal. Therefore, how to correctly and quickly find out the type of the skin lesion is very important. From this inspiration, we are interested in exploring the use of machine learning algorithms to aid medical professionals in the diagnosis skin lesions. To help explore the usage of the machine learning models, we used HAM10000 dataset from Harvard which it contains seven types of the skin lesions. This project is referencing to the paper: Soft-Attention Improves Skin Cancer Classification Performance. In this github, we would show how to pre-processed raw dataset and how we use VGG16, ResNet50 with transfer learning and from scratch.



<a name="methodologyandresults"></a>
## Methodology and Results
In this project, we mainly used Convolution Neural Network models:
- VGG16: Transfer Learning, built from strach
- ResNet50: Transfer Learning, built from strach

All the results we got is showing below:



<a name="datasource"></a>
## Data Scource






<a name="code"></a>
## Code

### Data Analysis
- [pre_processing.py](../master/src/pre_processing.py) : Data loading, cleaning and pre-processing
- [analysis.py](../master/visualization/analysis.py) : Analysis tools, plots and visualizations
### Feature Extraction
- [feature_extraction.py](src/feature_extraction.py) : Feature extraction and preparing the data for ML models
### Prediction
- [prediction.py](src/prediction.py) : Prediction on the test data using Logistic Reg., XGBoost, and Random Forest models
### Dashboard
- [dashboard.py](dashboard.py) : Dash app of the product, includes all plots and capabilities of the dashboard
### Test Coverage Report 
- [generate_coverage_report.py](test/generate_coverage_report.py) : Generates [Test Coverage Report](test_coverage_report.pdf). Developed and tested on MacOS 10.15.3 (running on any other OS may require minor changes to the script).




<a name="filestructure"></a>
## File Structure

```
├── dataset
|   ├── bank-additional-full.csv
|   ├── bank-additional-full.csv
|   └── bank-additional.csv
├── src
|    ├── pre_processing.py
|    ├── feature_extraction.py
|    └── prediction.py
├── doc
|    ├── build
|    |   ├── doctrees
|    |   |    ├── environment.pickle
|    |   |    └── index.doctree
|    |   └── html
|    |   |    ├── _sources
|    |   |    ├── _static
|    |   |    ├── .buildinfo
|    |   |    ├── genindex.html
|    |   |    ├── index.html
|    |   |    ├── objects.inv
|    |   |    ├── py-modindex.html
|    |   |    ├── search.html
|    |   |    └── searchindex.js
|    ├── source
|    |   |    ├── conf.py
|    |   |    └── index.rst
|    ├── Makefile
|    └── make.bat
├── test
|    ├── generate_coverage_report.py
|    ├── test_analysis.py
|    ├── test_dashboard.py
|    ├── test_feature_extraction.py
|    ├── test_pre_processing.py
|    ├── test_prediction.py
|    └── test_util.py
├── visualization
|    ├── analysis.py
|    └── 229_plots.ipynb
├── Dockerfile
├── LR_prediction.joblib
├── README.md
├── dashboard.py
├── docker-compose.yml
├── requirements.txt
├── temp-plot.html
├── test_coverage_report.pdf
├── ECE229-presentation.pdf
└──  util.py
```

<a name="requirepackages"></a>
## Require Packages

- Python >=3.7
- dash
- dash-renderer
- dash-core-components
- dash-html-components
- dash-table
- plotly
- numpy
- pandas
- scipy
- matplotlib
- seaborn
- xgboost
- scikit-learn
- coverage
- pytest
- joblib

Run pip install -r requirements.txt to set up your computer. 



<a name="contributors"></a>
## Contributors


<a name="citation"></a>
## Citation
