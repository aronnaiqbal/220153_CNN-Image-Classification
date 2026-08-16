# 220153_CNN-Image-Classification

# CNN Image Classification using PyTorch

## Project Overview

This project implements a Convolutional Neural Network (CNN) using PyTorch for Rock-Paper-Scissors image classification. The model was trained on a standard Rock-Paper-Scissors dataset and evaluated using both standard test images and custom smartphone images captured by the user.

---
## Dataset Information

### Standard Dataset
Rock-Paper-Scissors Dataset

Classes:
- Paper
- Rock
- Scissors

Dataset Statistics:
- Training Images: 2520
- Test Images: 372

### Custom Dataset
For real-world testing, 10 custom smartphone images were captured and uploaded to GitHub.

Custom Classes:
- Paper
- Rock
- Scissors

---

## Data Preprocessing

The following preprocessing techniques were applied:

- Resize Images to 64 × 64
- Convert Images to Tensor
- Normalize Images using:

```python
mean = [0.5, 0.5, 0.5]
std = [0.5, 0.5, 0.5]
```

---

## CNN Architecture

The CNN model consists of:

- Conv2D (32 Filters)
- ReLU Activation
- Max Pooling

- Conv2D (64 Filters)
- ReLU Activation
- Max Pooling

- Conv2D (128 Filters)
- ReLU Activation
- Max Pooling

- Adaptive Average Pooling

- Fully Connected Layer (256 Neurons)
- Output Layer (3 Classes)

---

## Training Configuration

| Parameter | Value |
|------------|------------|
| Optimizer | Adam |
| Loss Function | CrossEntropyLoss |
| Epochs | 5 |
| Batch Size | 64 |
| Framework | PyTorch |

---

## Model Performance

| Metric | Value |
|----------|----------|
| Training Accuracy | 99.55% |
| Validation Accuracy | 100.00% |
| Test Accuracy | 88.17% |

---

# Results and Visualizations

## Loss vs Epochs
![Loss_vs_Epochs](https://github.com/aronnaiqbal/220153_CNN-Image-Classification/blob/602c80c2fcba2b29b1348c0e1abd76947e6add49/Screenshot/Loss_vs_Epochs.png)

---

## Accuracy vs Epochs
![Accuracy_vs_Epochs](https://github.com/aronnaiqbal/220153_CNN-Image-Classification/blob/749204a552fc780c21e90af5e82124fe26a35640/Screenshot/Accuracy_vs_Epochs.png)

---

## Confusion Matrix
![Confusion_Matrix](https://github.com/aronnaiqbal/220153_CNN-Image-Classification/blob/2462a87db67a7faaffe4955d6aca907f69a38f94/Screenshot/Confusion_Matrix.png)

---

## Custom Prediction Gallery

The trained CNN model was tested on 10 custom smartphone images.
![Custom_Prediction_Gallery](https://github.com/aronnaiqbal/220153_CNN-Image-Classification/blob/dd14d186d7c9c9ae2623cae7c4110a0c574e967f/Screenshot/Custom_Prediction_Gallery.png)

---

## Visual Error Analysis

Three randomly selected misclassified images from the standard test dataset.
![Visual_Error_Analysis](https://github.com/aronnaiqbal/220153_CNN-Image-Classification/blob/ae504d327348644f9032d9f4204808c5ca59f0c4/Screenshot/Visual_Error_Analysis.png)

---

## Repository Structure

```text
220153_CNN-Image-Classification
│
├── dataset
│   └── custom_images
│
├── images
│   ├── Loss_vs_Epochs.png
│   ├── Accuracy_vs_Epochs.png
│   ├── Confusion_Matrix.png
│   ├── Custom_Prediction_Gallery.png
│   └── Visual_Error_Analysis.png
│
├── model
│   └── 220153.pth
│
├── 220153.ipynb
│
└── README.md
```

---

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-Learn
- Google Colab
- GitHub

---

## Conclusion

This project demonstrates a complete CNN-based image classification workflow using PyTorch. The model achieved high training and validation accuracy on the Rock-Paper-Scissors dataset and was successfully evaluated on real-world smartphone images. The project covers dataset preprocessing, CNN model development, training, evaluation, visualization, and real-world testing.
