# UsiNet

UsiNet is designed for the unsupervised sinogram inpatining of nanoparticles electron tomography. Here two training examples are provided on computer simulated tilting series and experimentally obtained tilting series.  
Current version: 1.0  
Date: 2/2023  
Tested on Google Colab  
For more information about the project, algorithms, and related publications please refer to the Chen Group website.  

# Reference

If you find our UsiNet is helpful to your publication, please cite:

Lehan Yao, Zhiheng Lyu, Jiahui Li, Qian Chen, "Unsupervised Sinogram Inpainting for Nanoparticle Electron Tomography (UsiNet) for missing wedge correction" _npj Computation Materials_ 
# Getting started

1. Example data download  
Considering the limited space on GitHub, we provided the training datasets via Illinois Data Bank at:  
https://databank.illinois.edu/datasets/IDB-7963044?code=qcGj7ceW6dT1CGB6Okt9UW91Wp0hFvVaaxmBiTr3QUM  
Two zip folders "simulated_data.zip" (simulated dataset) and "experimental_data.zip" (experimental dataset) could be downloaded.
In each folder we provide an "image_data.zip" and a "training_data.zip". The former one are raw image data convenient for your visualization. The latter one contains the .npy files which will be used by the training codes.  
Both simulated dataset and experimental dataset contain train.npy (the training data) and test.npy (data to be predicted). Simulated dataset also contains valid.npy (validation data) and label.npy (validation ground truth).  
For your information: For the image_data.zip in simulated_data.zip, it contains 360 raw tilting series, where 1-300 are used as training data; 301-350 are validation data; and 351-360 are test data. For the image_data.zip in experimental dataset.zip, it contains 126 raw tilting series, where all of them are used as both training data and test data.  
2. Folder structures  
Please download the Jupyter Notebook codes and training data example and create output folders as following:  
|— trainingExample.ipynb  
|— train.npy  
|— valid.npy (for simulated dataset only)  
|— label.npy (for simulated dataset only)  
|— test.npy  
|— output  
&emsp;&emsp;|— 1st  
&emsp;&emsp;|— 2nd  
&emsp;&emsp;|— test_pred  
3. Model training  
Run trainingExample.ipynb for training  
A neural network model file and a training loss log file will be generated in the root folder of the script. The image outputs will be generated in the output folder.  
Little tips: The output sinogram stacks in test_pred can be conveniently switched to tilting series view with the Image/Stack/Reslice function in ImageJ. The output images might look oversaturated. But no worries, it's just a matter of dynamic range and can be fixed by the Image/Adjust/Brightness/Contrast function in ImageJ.
