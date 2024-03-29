# Detecting-Retinal-Damage-with-OCT-images
# Retinal OCT Image Classification

## Project Overview
This project leverages deep learning to automate the detection and classification of retinal diseases from Optical Coherence Tomography (OCT) images. Utilizing a dataset of less than 1,000 OCT images, we demonstrate the effectiveness of transfer learning with pretrained networks such as VGG16 and InceptionV3 to classify images into four categories: Normal, CNV (Choroidal Neovascularization), DME (Diabetic Macular Edema), and Drusen.

## Objective
The goal is to support ophthalmologists by automating the classification of OCT images, thus aiding in the diagnosis and treatment planning of retinal diseases. We aim for high accuracy to ensure reliability in clinical applications.

## Dataset
The dataset is sourced from "Identifying Medical Diagnoses and Treatable Diseases by Image-Based Deep Learning" by Kermany et al., 2018, available publicly. It comprises OCT images categorized into Normal, CNV, DME, and Drusen classes.

## Methodology
1. **Data Preparation**: Loading and preprocessing OCT images, including resizing and normalization.
2. **Data Visualization**: Visualizing the dataset to understand the class distribution.
3. **Model Development**: Employing transfer learning with VGG16 and InceptionV3, customized for OCT image classification.
4. **Training and Evaluation**: Models are trained and evaluated on the dataset using metrics such as accuracy, precision, recall, and f1-score. Analysis is supported by confusion matrices and learning curves.
5. **Optimization and Testing**: Implementing data augmentation and undersampling to optimize performance and address class imbalance.

## Results
The project achieves an accuracy rate of approximately 95% in classifying OCT images, indicating high potential for clinical application. Efforts to further improve performance are ongoing.

## Future Work
- Enhancing model accuracy towards 99%.
- Incorporating data augmentation for better generalization.
- Analyzing model performance with ROC curves.
- Exploring interpretability features such as Grad-CAM.

