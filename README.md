# UsiNet

UsiNet is designed for the unsupervised sinogram inpatining of nanoparticles electron tomography. Here two training examples are provided on computer simulated tilting series and experimentally obtained tilting series.  
Current version: 1.0  
Date: 2/2023  
Tested on Google Colab  
For more information about the project, algorithms, and related publications please refer to the Chen Group website.  

# Reference

If you find our statistical approach useful for analyzing your data, please cite:

Lehan Yao, Zhiheng Lyu, Jiahui Li, Qian Chen, "Unsupervised sinogram inpainting for missing wedge artifacts correction in heterogeneous nanoparticle electron tomography" _npj Computation Materials_ 
# Getting started

1. Example data download  

2. Folder structures  
|— trainingExample.ipynb  
|— train.npy  
|— valid.npy  
|— label.npy  
|— test.npy  
|— output  
&nbsp;|— 1st  
&nbsp;|— 2nd  
&nbsp;|— test_pred  
3. Model training  
