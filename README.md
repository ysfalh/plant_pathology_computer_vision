# Plant pathology diagnosis: A computer vision application
Please read the project report available in main directory to find out more about the subject and how we approach it.

This project is based on a scientific publication [[1]](#1) and a Kaggle competition [[2]](#2) that took place from March 9 to
May 26, 2020.

### References
<a id="1">[1]</a> 
Ranjita Thapa, Noah Snavely, Serge Belongie, and Awais Khan. 
The plant pathology 2020 challenge dataset to classify foliar disease of apples, 2020.

<a id="2">[2]</a> 
Kaggle - plant pathology 2020 - Link : https://www.kaggle.com/c/plant-pathology-2020-fgvc7/overview.

## How to use the code

The code associated with the project is organized as follows:
- Data augmentation (from images directly, locally): data_augmenting.py
- Creation of datasets (from previous images stored at the following git - https://gitlab.binets.fr/paul.calot-plaetevoet/plantpathology_2020.git): creatingDatasets.ipynb
- Development of architectures. The selected notebooks are as follows:
  - resnet50.ipynb
  - googlenet.ipynb
  - vgg16.ipynb
  - efnetb3.ipynb
  - processing_resnet50_definitive.ipynb
  - processing_resnet50_3classes.ipynb

A drive with the following datasets, in torch.dataset format, is also available at the following address: https://drive.google.com/drive/folders/1xTUMQhu-JbkTSriWoLJxmJXrj5jnrKym?usp=sharing

- Testing sets:
  - testing_set_3classes
  - testing_set_1400 (77-23% split)
  - testing_set_60 (60-40% split)

- Training sets:
  - dataset_8 (77-23% split)
  - dataset_4 (77-23% split)
  - dataset_6 (60-40% split)
  - dataset_3classes (77-23% split)
  - dataset_0 (77-23 split)

Whether on the git or on the drive, not all the datasets created are available: for reasons of available memory, we have only put the most relevant.
