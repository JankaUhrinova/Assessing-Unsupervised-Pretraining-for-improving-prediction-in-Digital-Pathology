# Assessing-Unsupervised-Pretraining-for-improving-prediction-in-Digital-Pathology

The code that handles the main part of the project is stored in two .ipynb notebooks. One handles the evaluation of pretraining methods and the other evaluates DCGAN.

How to run the code in all_methods_comparison.ipynb:

This notebook contains cell that handle pretraining of an AutoEncoder, retraining of the Encoder, training of a pretrained Clasifier and training of a non-pretrained classifier and testing. If you only want to run some parts it is necessary to set corresponding flags to True at the begining of the notebook. If all parts are run, the process can take several hours.

The folder that contains code also contains every pretrained and trained model used for the evaluation. 
They can be stored on an arbitrary place your notebook can get access to. Since I was using Google Colab, I stored them on my personal Drive.
The dataset can be downloaded on the following site https://zenodo.org/record/1214456 (it is important to download normalized dataset).
The dataset also needs to be stored at the place that notebook will have access to. 
Once the place for dataset and models is chosen it is necessary to replace all paths used in the code. 
These places are indicated with text cells that tell you what path to use as a replacement.


How to run the code in DCGAN_100K.ipynb:

This notebook will train DCGAN on 20000 random images from a 100K dataset. Handling the dataset is identical to how it is done all_methods_comparison.ipynb
There are no pretrained models or flags in this notebook so changing the paths for the dataset should suffice for the notebook to run successfuly. 

The whole training process can take up to 7 hours on GPU.
 