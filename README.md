# ECE228-Group37 Skin Lesion Classification
![dashboard_preview](/Results/backgroud_image.jpeg)
---
## Table of Content
- [Introduction](#introduction)
- [Methodology and Results](#methodologyandresults)
- [Data Source](#datasource)
- [Code and Result Plots](#code)
- [File Structure](#filestructure)
- [Require Packages](#requirepackages)
- [How to Run Codes to Generate Same Result](#run)
- [Contributors](#contributors)


<a name="introduction"></a>
## Introduction
There are many types of the skin lesion. Some of the them are not fatal and can be cured with appropriate treatment. However, some of them are actually cancer and they are fatal. Therefore, how to correctly and quickly find out the type of the skin lesion is very important. From this inspiration, we are interested in exploring the use of machine learning algorithms to aid medical professionals in the diagnosis skin lesions. To help explore the usage of the machine learning models, we used HAM10000 dataset from Harvard which it contains seven types of the skin lesions. This project is referencing to the paper: Soft-Attention Improves Skin Cancer Classification Performance. In this github, we would show how to pre-processed raw dataset and how we use VGG16, ResNet50 with transfer learning and from scratch.
The report can be found here: 
[report](/Results/ECE228_Final_Report.pdf)



<a name="methodologyandresults"></a>
## Methodology and Results
In this project, we mainly used Convolution Neural Network models:
- VGG16: Transfer Learning, built from strach
- ResNet50: Transfer Learning, built from strach

All the results we got is showing below:
![result](/Results/score_table.png)


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

Since the dataset is so large, even a zip file can not be uploaded to Github. Please follow instructions to complete data pre-processing.



<a name="code"></a>
## Code and Result Plots

### Data Analysis
- [Pre_processing.py](../main/Data%20Pre-processing/Pre_processing.ipynb) : Dataset geneartion of two Zips from [dataset link](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T)
- [Generate Image for Poster .ipynb](../main/Data%20Pre-processing/Generate%20Image%20for%20Poster%20.ipynb) : Generate 7 skins lesion image example for poster section
### Models Build from Scratch
- [ResNet50_Scratch.ipynb](Build%20From%20Scratch/ResNet50_Scratch.ipynb) : ResNet50 build from scratch
- [VGG16.ipynb](Build%20From%20Scratch/VGG16.ipynb) : VGG16 build from scratch
### Transfer Learning Models
- [ResNet50_Transfer.ipynb](Transfer%20Learning/ResNet50_Transfer.ipynb) : ResNet50 Transfer Learning
- [VGG16_TransferLearning.ipynb](Transfer%20Learning/ResNet50_Transfer.ipynb) : VGG16 Transfer Learning
### Result Plots
- [Res50_T_a.png](Results/Res50_T_a.png) : ResNet50 Transfer Learning Accuracy Plot
- [Res50_T_l.png](Results/Res50_T_a.png) : ResNet50 Transfer Learning Loss Plot
- [Res50_S_acc.png](Results/Res50_S_acc.png) : ResNet50 build from scratch Accuracy Plot
- [Res50_S_loss.png](Results/Res50_S_loss.png) : ResNet50 build from scratch Loss Plot
- [V16_tran_acurracy.png](Results/V16_tran_acurracy.png) : VGG16 Transfer Learning Accuracy Plot
- [V16_tran_loss.png](Results/V16_tran_loss.png) : VGG16 Transfer Learning Loss Plot
- [VGG16_accuracy.png](Results/VGG16_accuracy.png) : VGG16 build from scratch Accuracy Plot
- [VGG16_loss.png](Results/VGG16_loss.png) : VGG16 build from scratch Loss Plot
- [score_table.png](Results/score_table.png) : Metric Evaluation scores for 4 models





<a name="filestructure"></a>
## File Structure

```
????????? Build From Scratch
|   ????????? ResNet50_Scratch.ipynb
|   ????????? VGG16.ipynb
|
????????? Data Pre-processing
|    ????????? Generate Image for Poster .ipynb
|    ????????? Pre_processing.ipynb
|
????????? Transfer Learning
|    ????????? ResNet50_Transfer.ipynb
|    ????????? VGG16_TransferLearning.ipynb
|
|__ Results
|    ????????? Res50_T_a.png
|    ????????? Res50_T_l.png
|    ????????? Res50_S_acc.png.ipynb
|    ????????? Res50_S_loss.png.ipynb
|    ????????? V16_tran_acurracy.png
|    ????????? V16_tran_loss.png
|    ????????? Res50_S_loss.png.ipynb
|    ????????? V16_tran_acurracy.png
|    ????????? V16_tran_loss.png
|    ????????? VGG16_accuracy.png
|    ????????? VGG16_loss.png
|    ????????? score_table.png
|
????????? README.md
????????? requirements.txt


```

<a name="requirepackages"></a>
## Require Packages

- Python >=3.8
- tensorflow 
- scikit-learn



Run pip install -r requirements.txt to set up your computer. 

<a name="run"></a>
## How to Run Codes to Generate Same Result 
1. Download the dataset from [dataset link](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T).
2. Install all required packages.
3. Use [Pre_processing.py](../main/Data%20Pre-processing/Pre_processing.ipynb) to generate the same training&testing dataset with each one has 7 sub-directories names as each skin lession. Change the  file path correspondingly, the code given is using the path locally! This is very important, please make it the same way as described! Otherwise, all codes won't run well!
5. Try 4 different models and generate the result. You can compare it with all figures we have, there will be a small difference. If a image corrupted, please find its path and delete it, otherwisem the model will stop learn. Image corruption happens sometimes when unzipping!


<a name="contributors"></a>
## Contributors
![contributors](/Results/Contributor.jpeg)
This project finished by two members: Xingtong Yang(left) and Zhiyin Liu (right)


