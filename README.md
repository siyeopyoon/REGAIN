# Resolution-Enhancement-Generative-Adversarial-Inline-Network (REGAIN)

The repository contains a source code for Resolution-Enhancement-Generative-Adversarial-Inline-Network (REGAIN). REGAIN is a generative adversarial neural network for REGAINing image sharpness and Spatial resolution. The trained network generates a resolution-enhanced image in the Phase-encoding (ky) direction in MRI.

## Requirements

For training and testing: torch, numpy


For GUI-based testing: torch, numpy, scipy, PyQt5, pydicom,  PIL, qimage2ndarray, opencv-python

## Pretrained Model and Reconstructed Results 

### Pretrained Model 
The pretrained model can be found at Dataverse of ANNONYMIZED (ANNONYMIZED).
Please refer file name "Pretrained_Model_REGAIN_epoch500-1.pth".


### Reconstructed Results
The testing result from 181 patients can be found at Dataverse of ANNONYMIZED (ANNONYMIZED). The results present reconstructed image data 1) Breath-hold GRAPPA-accelerated ECG-gated segmented Cine 2) Free-breathing CS-accelerated Real-time Cine

## File Descriptions
-Config.py: The configuratioFile Descriptionsn file for defining a cuda machine, dataroot folder, and hyperparameters during training

-Dataset.py: Specefies the training dataset loading and data augumentation

-Models.py: Implementation of REGAIN

-Train.py: The numpy magnitude images are loaded and the training is performed. (This is what you run for training)

-Test.py: The numpy magnitude images are loaded and the testing is performed. (This is what you run for testing)

-GUI-Testing.py: The DICOM files are loaded and visualize the result of REGAIN (This is what you run for off-line Reconstruction)

