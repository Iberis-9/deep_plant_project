# 🌿 Plant Classification with EfficientNetB0

## Overview

This project explores building an image classification model capable of identifying a small set of common household plants from photographs. The model is based on **EfficientNetB0** and uses transfer learning to adapt a pre-trained convolutional neural network to this specific task.

The broader goal is to lay the foundation for a simple application where users could upload a plant image and receive a predicted plant species along with basic care guidance.

---

## Model Approach

- **Architecture:** EfficientNetB0 (pre-trained on ImageNet)
- **Transfer Learning:** Frozen base layers with light fine-tuning
- **Train/Validation Split:** 80/20
- **Image Size:** 224 × 224
- **Batch Size:** 32

---

## Results

The model performs well on validation data and achieves solid accuracy on clear, well-framed images.

However, testing on new real-world images revealed inconsistent predictions when plants were photographed from unusual angles, under varied lighting conditions, or when their appearance differed from typical training examples. This highlights the importance of dataset size and diversity for improving model generalization.

---

## Dataset

The dataset is not included in this repository due to size and licensing considerations.  
Images were collected from publicly available sources for educational purposes.


To run this project locally, create the following folder structure:

plant_classification_project/
│
├── notebook.ipynb
├── plants_data/
│ ├── monstera/
│ ├── zamioculcas/
│ ├── alocasia/
│ └── ...

Each subfolder should contain images of the corresponding plant class.

---

## Future Improvements

- Increase dataset size and diversity  
- Apply stronger data augmentation  
- Further fine-tune the model  
- Deploy as a simple web application  

---

## Tech Stack

- Python  
- TensorFlow / Keras  
- EfficientNetB0  
- Matplotlib  
