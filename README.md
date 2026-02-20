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
  <img width="642" height="107" alt="image" src="https://github.com/user-attachments/assets/faef3e82-9c45-4e40-94dc-d91a481412f3" />


Quantization preserved model accuracy while significantly reducing size, enabling embedded deployment.

----
## TensorFlow Lite Conversion

The trained model was converted using full INT8 quantization with a representative dataset to ensure proper calibration.

Key steps:

- Optimize.DEFAULT

- Representative dataset

- INT8 input/output

- Accuracy evaluation with quantization scaling

----

## Confusion Matrix
<img width="437" height="384" alt="image" src="https://github.com/user-attachments/assets/aa8a5abb-b2e9-43f5-b382-8e8856daaddc" />


----
## Future Work

- Dynamic gesture recognition (temporal modeling)

- Real-time hardware deployment (ESP32 / STM32)

- Model pruning

- Mixed precision inference

- Larger dataset with varied environmental conditions

----
🧑‍💻 Author

Jonathan Mishayel

Research Project | Embedded AI & TinyML

@2025
