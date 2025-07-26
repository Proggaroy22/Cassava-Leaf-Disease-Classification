# Cassava-Leaf-Disease-Classification

**Dataset Source:** https://www.kaggle.com/competitions/cassava-leaf-disease-classification

**Classes**:

Cassava Bacterial Blight (CBB)

Cassava Brown Streak Disease (CBSD)

Cassava Green Mottle (CGM)

Cassava Mosaic Disease (CMD)

Healthy Leaves

**Experimental Models (CNN)**:

ResNet-150

ResNet-50

DenseNet-121

EfficientNet-B0

EfficientNet-B3

**Experimental Models (Transformers):**

EfficientNeViT-b3

ViT

**Data Augmentation:**

**Augmentation techniques in the training set:**

Resize

Random horizontal flips

Random Rotations

ColorJitter (brightness=0.2, contrast=0.2, saturation=0.2)

Normalization based on ImageNet mean and std

**Augmentation techniques for validation/test set:**

Only includes resizing, tensor conversion, and normalization.

No augmentation to ensure consistent evaluation.

Split Ratio:   Train: Test: Validation: 70:15:15

**Class distribution in training set:**

Class 4: 2061 samples

Class 3: 10526 samples

Class 1: 1751 samples

Class 2: 1909 samples

Class 0: 870 samples

**Class Balancing via Oversampling:**

Random sampling with replacement for oversampling. As a result, the final training dataset is class-balanced, improving the model’s ability to learn equally from all classes and reducing classification bias.

**Training Details:**

Loss Function: CrossEntropyLoss

Optimizer: Adam

Early Stopping: Enabled

Training Epochs: 100

Patience Count: 05

**Evaluation Metrics Computed:**

Accuracy

Precision (Weighted)

Recall (Weighted)

F1 Score (Macro Average)

AUC-ROC 
