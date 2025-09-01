# Pneumonia Detection Using CNN
## Overview
This project focuses on detecting pneumonia in chest x-ray scans using convulutional neural networks. Pneumonia is a serious infection which can be life threatening especially in vunerable populations. 

Through training on a public chest scan dataset, this model is able to distinguish between pneumonia-infected and healthy lungs with a F1-score of 90. Demonstrating how this technology can be used to help medical professionals provide faster and more accurate diagnoses.

## Features
* Automated pneumonia detection from X-ray images
* Model trained using Kaggle dataset
* Able to achieve an F1 score of 90
* Runs fully on cloud

## Tech Stack
* **Language:** Python
* **Frameworks/Libraries:** Tensorflow, Keras, Matplotlib
* **Dataset:** https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

## Results
Initial runs running on a handmade model resulted in high accuracy, yet failed to perform when running on independent data. Achieving accuracy in the 60s yet having 100% accuracy during training.

<img width="584" height="455" alt="pneuacc1" src="https://github.com/user-attachments/assets/861012f8-181f-4d9a-86b1-08f7357f8ced" />


Through modifying the models layers to bettter handle the inputs, adding callbacks, and augmenting the training data the models overfitting dropped. Yet still only performed in the 80s.

<img width="576" height="455" alt="pneuacc2" src="https://github.com/user-attachments/assets/2b252eed-cfad-4545-bc85-ea28e35a6fb9" />


The final push in accuracy was achieved using transfer learning and fine tuning. By leveraging the EfficientNetB0 architecture and fine-tuning techniques, the model is able to achieve an accuracy of 90%. While also cutting the parameters in half, improving training time and compute usage.

<img width="539" height="432" alt="download" src="https://github.com/user-attachments/assets/1df27604-2d43-4142-90a5-a621a91b0f78" />
