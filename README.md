# Diabetic-Ratinopathy

## Abstract

Diabetic retinopathy, a common eye disorder among individuals with diabetes, is a leading cause of blindness. This project employs neural networks and deep learning techniques, including Faster CNN and Resnet50, to detect anomalies in retinal images associated with diabetic retinopathy. The goal is to aid ophthalmologists in identifying abnormalities like hemorrhage, exudates, and macula. The project includes a live demo available [here](#).

## Introduction

Diabetic retinopathy diagnosis and treatment depend on the severity of retinal vascular disease observed during ophthalmoscopy. The project classifies diabetic retinopathy into three types: Non-Proliferative diabetic retinopathy, Progressive accumulation of microvascular change, and Retinal capillary nonperfusion. Diabetic retinopathy is a significant cause of blindness, especially among working-age adults.

## Methods

The initial methodology involved creating a Convolutional Neural Network (CNN) model using Kaggle's provided retinal images. The model was trained to detect macula formations and damaged blood cells. However, overfitting occurred due to uneven distribution and data augmentation. To address this, an attention mechanism was introduced using Resnet50 with a masking layer to enhance macula detection. The dataset, containing high-resolution retinal images, was rated by clinicians on a scale of 0 to 4 based on the presence of diabetic retinopathy.

### Data Set Details:

- Approximately 25K high-resolution retinal images.
- Clinician ratings: 0-NoDR, 1-Mild, 2-Moderate, 3-Severe, 4-Proliferative DR.

### Identify the Main Study Variables:

The main focus was on the macula and optic nerves disorders, indicating retina damage and cancerous blood cell formation. Attention mapping with Resnet50 and CNN model was utilized to achieve accurate predictions.

### Data Collection Instruments and Procedures:

Data obtained from Kaggle contained 25K high-resolution images with varying distributions of DR. Data augmentation was applied to achieve uniform distribution, and an attention architecture was implemented for accurate predictions.

## Results

The model performance on the test set showed overfitting due to data augmentation. The confusion matrix revealed the model's struggle to predict severe and Proliferative DR. The AUC graph indicated convergence, but the model's overall performance was not satisfactory.

## Conclusions and Future Work

The challenges include feeding entire retinal images into deep networks due to resource constraints. Further research is needed to explore kernels of variable sizes for image slicing, preventing loss of crucial information. Deep learning models' performance should be validated in real-time clinical examinations. Collaboration with expert ophthalmologists is crucial for developing and validating intelligent systems.

