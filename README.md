# Vehicle Damage Assessment System

## Project Overview
This project implements a deep learning–based Vehicle Damage Assessment System as part of the Pattern Recognition Project (Part 2). The objective is to automatically classify vehicle damage severity from images into four categories: no damage, minor, moderate, and severe.

The system uses Convolutional Neural Networks (CNNs) and transfer learning techniques to achieve accurate, interpretable, and robust vehicle damage classification. The project investigates baseline model performance, architectural comparisons, the impact of data augmentation, model interpretability, and robustness under varying lighting conditions.

---

## Dataset Source
The dataset consists of labeled vehicle images categorized by damage severity. Images are organized into training, validation, and test sets. The dataset was preprocessed and resized before being used for model training and evaluation.

### Folder Structure
data/
├── train/
├── val/
└── test/

Each split contains the following classes:
- no_damage
- minor
- moderate
- severe

---

## Model Architecture
The following deep learning models are evaluated in this project:

- **Base CNN**: A custom convolutional neural network built from scratch using convolutional, max-pooling, and fully connected layers.
- **ResNet50**: A deep residual network implemented using transfer learning.
- **MobileNetV2**: A lightweight and efficient CNN architecture suitable for resource-constrained environments.

To improve generalization, data augmentation techniques such as rotation, zoom, and horizontal flipping are applied. Model interpretability is analyzed using Gradient-weighted Class Activation Mapping (Grad-CAM), which highlights image regions influencing the model’s predictions.

---

## Experiments and Research Questions
The project addresses the following research questions:

- **RQ1**: Performance of a baseline CNN for vehicle damage classification  
- **RQ2**: Comparison of different CNN architectures  
- **RQ3**: Impact of data augmentation on performance  
- **RQ4**: Model interpretability using Grad-CAM  
- **RQ5**: Robustness under varying lighting conditions  

All figures and tables related to these research questions are provided separately in `Figures_Tables.zip`.

---

## Instructions to Reproduce Results

### 1. Clone the repository
```bash
git clone https://github.com/Naveen0713/Vehicle-Damage-Assessment-System.git
cd Vehicle-Damage-Assessment-System

2. Create and activate a virtual environment
python3 -m venv venv
source venv/bin/activate

3. Install required dependencies
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow torchvision opencv-python openpyxl

4. Prepare the dataset
Place the dataset inside the data/ directory following the folder structure described above.

5. Run the notebook
jupyter notebook

Open the notebook:
Vehicle_Damage_Assessment.ipynb

Then run:
Kernel → Restart Kernel → Run All

Repository Contents
Vehicle_Damage_Assessment.ipynb – Complete implementation and experiments
README.md – Project documentation
Figures_Tables.zip – Final figures and tables (submitted separately)

Authors
Student 1 – Technical Lead
Student 2 – Figures and Tables
Student 3 – Report and Interpretation

Notes
This repository is intended for academic use only and follows the submission guidelines for the Pattern Recognition Project (Part 2).
