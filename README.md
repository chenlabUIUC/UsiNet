# UsiNet

UsiNet is designed for the unsupervised sinogram inpatining of nanoparticles electron tomography. Here two training examples are provided on computer simulated tilting series and experimentally obtained tilting series.  
Current version: 1.0  
Date: 2/2023  
Tested on Google Colab  
For more information about the project, algorithms, and related publications please refer to the Chen Group website.  

# Reference

If you find our UsiNet is helpful to your publication, please cite:

Lehan Yao, Zhiheng Lyu, Jiahui Li, Qian Chen, "Unsupervised sinogram inpainting for missing wedge artifacts correction in heterogeneous nanoparticle electron tomography" _npj Computation Materials_ 
# Getting started

1. Example data download  
Considering the limited space on GitHub, we provided the training datasets via Illinois Data Bank.  
Both simulated dataset and experimental dataset contain train.npy (the training data) and test.npy (data to be predicted). Simulated dataset also contains valid.npy (validation data) and label.npy (validation ground truth).
2. Folder structures  
Please download the Jupyter Notebook codes and training data example and create output folders as following:  
|— trainingExample.ipynb  
|— train.npy  
|— valid.npy  
|— label.npy  
|— test.npy  
|— output  
&emsp;&emsp;|— 1st  
&emsp;&emsp;|— 2nd  
&emsp;&emsp;|— test_pred  
3. Model training  
Run trainingExample.ipynb for training  
A neural network model file and a training loss log file will be generated in the root folder of the script. The image outputs will be generated in the output folder.  
