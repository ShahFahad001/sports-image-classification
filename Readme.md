# Sports Image Classification using ResNet-50

This is my capstone project for the course **INFO-6147: Deep Learning with PyTorch** at Fanshawe College.
In this project, I used a **pretrained ResNet-50 model** to classify images into 7 different sports categories using transfer learning.

---

##  Dataset

- **Dataset Name**: Sports Image Dataset
- **Classes**:
  - Badminton
  - Cricket
  - Karate
  - Soccer
  - Swimming
  - Tennis
  - Wrestling
- **Size**: ~8,300 images
- The data was balanced and each sport had clearly visible actions or uniforms.

---

##  Project Goals

- Train a CNN using real-world sports images
- Apply **transfer learning** using ResNet-50
- Perform **hyperparameter tuning** using Grid Search
- Evaluate model using accuracy, precision, recall, F1-score, and confusion matrix
- Share results in a report and presentation

---

##  Techniques Used

- PyTorch and Torchvision
- Transfer Learning with **ResNet-50**
- Early Stopping (Patience = 3)
- Grid Search for tuning:
  - Learning Rate
  - Batch Size
  - Optimizer (SGD, Adam)
- Data Augmentation:
  - Random Horizontal Flip
  - Random Rotation
  - Random Resized Crop

---

## Final Results

- **Best Validation Accuracy**: 89.80%
- **Final Test Accuracy**: **89.64%**
- **Best Performing Classes**:
  - Swimming (F1-Score: 0.97)
  - Wrestling (F1-Score: 0.94)
- **Challenging Class**:
  - Karate (confused with Wrestling)

---

## Project Files

| File Name                             | Description                                |
|--------------------------------------|--------------------------------------------|
| `Project_Code.ipynb`                 | Final Colab notebook with complete model   |
| `Final_Report.pdf`                   | Technical report with all results          |
| `Deep_Learning_Project_Presentation.pptx` | Final presentation slides               |
---

## How to Run (Google Colab)

1. Open `Project_Code.ipynb` in Google Colab
2. Make sure to upload the dataset or mount Google Drive
3. Install required libraries using:
   ```python
   !pip install torch torchvision scikit-learn matplotlib

