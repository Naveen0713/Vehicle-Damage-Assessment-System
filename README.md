# Vehicle Damage Assessment System

## Project Overview
This project implements a deep learning–based Vehicle Damage Assessment System as part of the Pattern Recognition Project (Part 2). The objective is to automatically classify vehicle damage severity from images into four categories: no damage, minor, moderate, and severe.

Convolutional Neural Networks (CNNs) and transfer learning techniques are used to achieve accurate, interpretable, and robust vehicle damage classification. The project evaluates baseline performance, compares different CNN architectures, studies the impact of data augmentation, analyzes model interpretability, and tests robustness under varying lighting conditions.

---

## Dataset Source
The dataset consists of labeled vehicle images categorized by damage severity. Images are divided into training, validation, and test sets to ensure unbiased evaluation.

Each dataset split contains the following classes:
- no_damage  
- minor  
- moderate  
- severe  

The dataset is organized using the following folder structure:
data/
├── train/
├── val/
└── test/

---

## Model Architecture
Multiple CNN-based models are implemented and evaluated in this project:

- **Base CNN**: A custom convolutional neural network built from scratch using convolutional, pooling, and fully connected layers.
- **ResNet50**: A deep residual network implemented using transfer learning to improve feature extraction.
- **MobileNetV2**: A lightweight and efficient CNN architecture designed for faster inference.

To improve generalization, data augmentation techniques such as rotation, zoom, and horizontal flipping are applied. Model interpretability is analyzed using Gradient-weighted Class Activation Mapping (Grad-CAM), which highlights image regions that influence model predictions.

---

## Instructions to Reproduce Results

1. Clone the GitHub repository:
git clone https://github.com/Naveen0713/Vehicle-Damage-Assessment-System.git
cd Vehicle-Damage-Assessment-System

2. Create and activate a virtual environment:
python3 -m venv venv
source venv/bin/activate

4. Install the required dependencies:
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow torchvision opencv-python openpyxl
5. Prepare the dataset:
Place the dataset inside the data/ directory following the folder structure described above.

7. Run the Jupyter Notebook:
jupyter notebook

Open Vehicle_Damage_Assessment.ipynb and run all cells from top to bottom:
Kernel → Restart Kernel → Run All

This will reproduce all experiments, evaluations, figures, and tables.

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
