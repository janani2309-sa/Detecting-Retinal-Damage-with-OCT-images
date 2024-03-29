# Detecting-Retinal-Damage-with-OCT-images
# Retinal OCT Image Classification

## Project Overview
This project leverages deep learning to automate the detection and classification of retinal diseases from Optical Coherence Tomography (OCT) images. Utilizing a dataset of less than 1,000 OCT images, we demonstrate the effectiveness of transfer learning with pre-trained networks such as VGG16 and InceptionV3 to classify images into four categories: Normal, CNV (Choroidal Neovascularization), DME (Diabetic Macular Edema), and Drusen.

## Objective
The goal is to support ophthalmologists by automating the classification of OCT images, thus aiding in the diagnosis and treatment planning of retinal diseases. We aim for high accuracy to ensure reliability in clinical applications.

## Dataset
The dataset is sourced from "Identifying Medical Diagnoses and Treatable Diseases by Image-Based Deep Learning" by Kermany et al., 2018, available publicly. It comprises OCT images categorized into Normal, CNV, DME, and Drusen classes.
Kindly find the dataset here - https://www.kaggle.com/code/janani2309/detect-retina-damage-from-oct-images/input


## Methodology
1. **Data Preparation**: Loading and preprocessing OCT images, including resizing and normalization.
2. **Data Visualization**: Visualizing the dataset to understand the class distribution.
3. **Model Development**: Employing transfer learning with VGG16 and InceptionV3, customized for OCT image classification.
4. **Training and Evaluation**: Models are trained and evaluated on the dataset using metrics such as accuracy, precision, recall, and f1-score. Analysis is supported by confusion matrices and learning curves.
5. **Optimization and Testing**: Implementing data augmentation and undersampling to optimize performance and address class imbalance.

## VGG16
#### Feature Extraction: 
VGG16, known for its simple and uniform architecture, excels at extracting low-level features such as edges and textures due to its deep stack of convolutional layers. In the context of OCT images, these features can be crucial for identifying subtle differences between normal tissues and pathological signs like fluid build-ups or membrane formations.
#### Transfer Learning Base: 
By using VGG16 as a feature extractor and adding custom layers on top, your project can fine-tune the model to specifically recognize patterns and anomalies present in retinal OCT images. This approach significantly reduces the training time and the amount of data required to achieve high accuracy.
Benchmarking: Given its widespread use and success in image classification tasks, VGG16 serves as a solid benchmark. Comparing its performance on your OCT dataset with other models can provide insights into the complexity and uniqueness of the task at hand.

## InceptionV3
#### Complex Feature Capture: 
The InceptionV3 architecture, with its inception modules, is designed to capture information at various scales using parallel convolutions. This ability makes it particularly effective for OCT image classification, where signs of retinal diseases might be visible at different sizes and resolutions.
#### Efficiency and Accuracy: 
InceptionV3 is known for its balance between computational efficiency and depth, allowing it to run relatively fast without sacrificing performance. This characteristic is beneficial for processing medical images, where model deployment in clinical settings demands both precision and speed.
#### Advanced Transfer Learning: 
Leveraging InceptionV3’s more advanced and diversified feature extraction capabilities compared to VGG16, your project can benefit from a nuanced understanding of OCT images. This is especially useful for distinguishing between closely related conditions like CNV and DME, which may share common features but have distinct characteristics crucial for accurate classification.
Integrating VGG16 and InceptionV3

## Comparative Analysis
By employing both VGG16 and InceptionV3, your project not only takes advantage of their respective strengths but also enables a comparative analysis of their performance on the same dataset. This comparison can guide the selection of the most suitable model or the development of an ensemble approach.
Adaptability and Scalability: The use of these models facilitates adaptability and scalability in your project. Depending on the evolving needs of the dataset or the introduction of new classes of retinal diseases, the models can be further fine-tuned or retrained with additional data.

In summary, VGG16 and InceptionV3 play crucial roles in your project by providing a strong foundation for feature extraction and classification through transfer learning, enabling your project to achieve high accuracy in detecting and classifying retinal damage in OCT images. Their integration underlines the project’s robustness and adaptability, setting a solid groundwork for future enhancements and clinical applicability.


## Results
The project achieves an accuracy rate of approximately 95% in classifying OCT images, indicating high potential for clinical application. Efforts to further improve performance are ongoing.

## Future Work
- Enhancing model accuracy towards 99%.
- Incorporating data augmentation for better generalization.
- Analyzing model performance with ROC curves.
- Exploring interpretability features such as Grad-CAM.

