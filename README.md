 # 🪖 Military Hand Signal Recognition using TinyML

## Project Overview

This project presents an efficient embedded vision approach for recognizing a limited set of military hand signals using a lightweight deep learning model optimized for deployment on resource-constrained devices.

The model is trained using transfer learning with MobileNetV2 and converted to TensorFlow Lite (INT8) for embedded deployment.

## Objectives

- Design a lightweight CNN-based classifier

- Analyze training convergence and generalization

- Apply fine-tuning techniques

- Optimize model using INT8 quantization

- Evaluate deployment feasibility on embedded systems
----
## Dataset
- 1200 images

- 3 classes:

      ✓ Halt

      ✓ Freeze

      ✓ Pistol

- Images resized to 224 × 224

- Data augmentation applied during training
## Model Architecture

- Base Model: MobileNetV2 (Pretrained on ImageNet)

- Transfer Learning

- Fine-Tuning (freezing early layers)

- Regularization:

      ✓ L2 Regularization

      ✓ Dropout

      ✓ Batch Normalization

## Results
    <img width="372" height="136" alt="image" src="https://github.com/user-attachments/assets/4d082703-5865-405f-a03f-074e6e964109" />


Quantization preserved model accuracy while significantly reducing size, enabling embedded deployment.
