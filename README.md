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
![result](/score_table.png)


<a name="datasource"></a>
## Data Scource
We used the HAM10000 dataset which contains seven different types of the skin lesion, which are:
- Actinic keratoses (akiec)
- basal cell carcinoma (bcc)
- benign keratosis (bkl)
- dermatofibroma (df)
- melanoma (mel)
- melanocytic nevus (nv)
- vascular lesions (vasc)

We mainly used dataset:
- HAM10000_images_part_1.zip
- HAM10000_images_part_2.zip

The dataset can be found on:
[dataset link](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T)





<a name="code"></a>
## Code

### Data Analysis
- [Pre_processing.py](../main/Data%20Pre-processing/Pre_processing.ipynb) : Dataset geneartion of two Zips from [dataset link](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T)
- [Generate Image for Poster .ipynb](../main/Data%20Pre-processing/Generate%20Image%20for%20Poster%20.ipynb) : Generate 7 skins lesion image example for poster section
### Models Build from Scratch
- [ResNet50_Scratch.ipynb](Build%20From%20Scratch/ResNet50_Scratch.ipynb) : ResNet50 build from scratch
- [VGG16.ipynb](Build%20From%20Scratch/VGG16.ipynb) : VGG16 build from scratch
### Transfer Learning Models
- [ResNet50_Transfer.ipynb](Transfer%20Learning/ResNet50_Transfer.ipynb) : ResNet50 Transfer Learning
- [VGG16_TransferLearning.ipynb](Transfer%20Learning/ResNet50_Transfer.ipynb) : VGG16 Transfer Learning





<a name="filestructure"></a>
## File Structure

```
├── Build From Scratch
|   ├── ResNet50_Scratch.ipynb
|   └── VGG16.ipynb
|
├── Data Pre-processing
|    ├── Generate Image for Poster .ipynb
|    ├── Pre_processing.ipynb
|
├── Transfer Learning
|    ├── ResNet50_Transfer.ipynb
|    ├── VGG16_TransferLearning.ipynb
|
|__ Results
|    ├── ResNet50_Transfer.ipynb
|    ├── VGG16_TransferLearning.ipynb
|    ├── ResNet50_Transfer.ipynb
|    ├── VGG16_TransferLearning.ipynb
|    ├── ResNet50_Transfer.ipynb
|    ├── VGG16_TransferLearning.ipynb
|
├── README.md
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
