# Counterfeit IC Detection System
---

## Overview
Counterfeit Integrated Circuits (ICs) pose a significant threat to industries like electronics manufacturing, telecommunications, and aerospace. This project presents a novel approach for counterfeit IC detection using a custom-designed **Convolutional Neural Network (CNN)**. By leveraging advanced data preprocessing techniques and architectural innovations, the proposed solution delivers high detection accuracy, enhancing the security and reliability of electronic systems.

---

## Problem Statement
The proliferation of counterfeit ICs jeopardizes the performance and safety of electronic devices. Traditional detection methods struggle to handle the complexities of modern counterfeit techniques. This project utilizes **deep learning** to analyze IC images and extract intricate features for robust counterfeit detection.

---

## Key Features
- **Custom CNN Architecture**: Combines elements of AlexNet and VGG16 for an optimal balance of performance and accuracy.
- **Data Augmentation**: Employs advanced techniques like random flips and rotations to improve model generalization.
- **High Accuracy**: Achieved a validation accuracy of **94%**, outperforming AlexNet and approaching VGG16's accuracy with reduced complexity.

---

## Dataset Description
1. **Classes**: Two classes - `Approved` and `Counterfeit`.  
2. **Size**: 85 images, augmented to 430 training and 17 validation samples.  
3. **Preprocessing**:
   - Resized images to dimensions of `(960, 720, 3)`.
   - Applied data augmentation techniques such as random rotations and flips.

---

## Methodology
1. **Baseline Models**:
   - **AlexNet**: Validation accuracy: 58.8%.  
   - **VGG16**: Validation accuracy: 70%, but with higher complexity.
2. **Proposed Model**:
   - 8 convolutional layers with ReLU activation, batch normalization, and max pooling.
   - Three fully connected layers for classification.
   - Optimized for reduced complexity and improved generalization.
3. **Training Details**:
   - **Optimizer**: Stochastic Gradient Descent (SGD).  
   - **Loss Function**: Cross-Entropy Loss.  
   - **Early Stopping**: Monitored validation loss with tolerance for stopping.

---

## Results
- **Validation Accuracy**: **94%**.  
- **Recall for Counterfeit Detection**: **86%**.  
- **Performance Comparison**:
  - **AlexNet**: Lower accuracy and insufficient complexity.  
  - **VGG16**: Comparable accuracy but higher computational overhead.  
  - **Proposed Model**: Optimal trade-off between accuracy and complexity.

---

## Future Work
1. **Additional Augmentation**:
   - Explore brightness and contrast adjustments for further generalization.
2. **Dropout Layers**:
   - Introduce dropout to reduce potential overfitting.
3. **Hyperparameter Optimization**:
   - Refine learning rates and other parameters for smoother training.
4. **Larger Dataset**:
   - Expand the dataset to include diverse counterfeit and approved ICs.

---

## How to Run the Project
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/counterfeit-ic-detection.git
   cd counterfeit-ic-detection
