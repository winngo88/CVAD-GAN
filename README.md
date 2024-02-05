# CVAD-GAN: Constrained video anomaly detection via generative adversarial network - CVAD_gan.ipynb 

This Jupyter notebook (`CVAD_gan.ipynb`) contains the implementation of a CVAD-GAN: Constrained video anomaly detection via generative adversarial network components. The notebook demonstrates the training of the model and provides functionalities for performing inference and visualizing results.

## Overview

The notebook implements a CVAE-GAN model, a hybrid architecture that combines the benefits of both Variational Autoencoders (VAEs) and Generative Adversarial Networks (GANs). This model is designed for image generation and anomaly detection.

Peds1 (#Video No.- 21)
<img src='Static/Ped1.gif' align="center" width="100%">
Peds2 (#Video No.- 4)
<img src='Static/Peds2.gif' align="center" width="100%">
Avenue (#Video No.- 12)
<img src='output1.gif' align="center" width="100%">

## Real Life Highway Video

** Note ** We are preparing a new dataset which is not mentioned in the manuscript which is still under Cleaning and adaption process as the purpose of this dataset to take Video Anomaly Detection Problems to Real-Time Video Detection And to Hardware Video Anomaly Detection. below is the result:- 
<img src='Static/file.gif' align="center" width="100%">

The Anomaly in this video is "Bike" going over the Divider which is a clear violation of the traffic rules which is considered as Anomaly and on basis of this we have identified some of the classes such as :
1. Cattels,

2. Wrong direction,

3. Slow/(Fast Speed exceed limit) Moving,

4. Person/Intruder,

5. Poor Visibility,

6. Fallen Object,

7. Stopped Vehicle

It is taken under some conditions such as only taking 5 frames per second out of 30 frames per second from the video. We are still trying to benchmark it on different models and other SOTA models such as :

1. STem-GAN
2. A2DGAN
3. VALDGAN
4. VALTGAN
5. MAAD GAN
6. AST NET




## Dependencies

- Python 3.8
- Jupyter Notebook
- TensorFlow
- Keras
- OpenCV
- Matplotlib
- Pillow

Install the dependencies using the following command:

```bash
pip install -r requirements.txt
```

## Usage
1. Open the Jupyter notebook:
```bash
jupyter notebook CVAD_GAN.ipynb
```
2. Execute the cells in the notebook sequentially.

3. Adjust hyperparameters, paths, or other configurations as needed.

## Training
Execute the cells related to model training to train the CVAD-GAN model. This involves loading the dataset, defining the model architecture, and training for a specified number of epochs.

## Inference
Execute the cells related to model inference to generate images and visualize results. This may involve loading a pre-trained model or using the trained model from the training phase.

## Results
View the generated images and anomaly detection results in the notebook. Optionally, save generated images in the img directory.

## File Structure
```bash
├── CVAD_GAN.ipynb               # Jupyter notebook for CVAD-GAN implementation
├── requirements.txt             # List of dependencies
├── img/                          # Directory to save generated images
├── models/                       # Directory to save trained models (if applicable)
├── dataset/                      # Directory containing the dataset
    ├── train/                    # Training data
    ├── test/                     # Testing data
```
