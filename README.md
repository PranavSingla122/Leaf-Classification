# Soybean Leaf Classification

## Overview
This project aims to classify soybean leaves into two categories: **Healthy** and **Yellow Mosaic**. It compares the performance of a **custom CNN** and **transfer learning using ResNet18**.

## Dataset
- The dataset consists of images of soybean leaves labeled as **Healthy** or **Yellow Mosaic**.
- The images are preprocessed with transformations like resizing, normalization, and data augmentation (random flips, rotations, and color jittering).

## Models Used
1. **Custom CNN Model:**
   - Two convolutional layers with ReLU activation and max pooling.
   - Fully connected layers with dropout to prevent overfitting.
   - Trained using Cross-Entropy Loss and Adam optimizer.

2. **Transfer Learning (ResNet18):**
   - Pretrained ResNet18 model with the final fully connected layer modified for 2-class classification.
   - Fine-tuned using Adam optimizer with weight decay.


## Results
| Model           | Train Accuracy | Validation Accuracy |
|---------------|---------------|-----------------|
| Custom CNN    | ~94%          | ~93%            |
| ResNet18 (TL) | ~99%          | ~98%            |

ResNet18 performed significantly better, leveraging pretrained features for improved accuracy.


## Contributions
Feel free to contribute by submitting issues or pull requests!
