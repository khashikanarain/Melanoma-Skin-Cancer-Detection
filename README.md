# Melanoma-Skin-Cancer-Detection
Melanoma is known as the most lethal form of skin cancer among the over 200 variants of the disease. Early diagnosis significantly increases treatment efficacy.
# Introduction
Melanoma skin cancer presents a critical health challenge due to its high mortality rate when
diagnosed late. Early detection through visual examination of affected skin areas and
subsequent analysis using dermatoscopic images is crucial. Despite advancements, the
traditional diagnostic process can be slow, taking up to a week or more from initial
consultation to biopsy results. This project leverages a Convolutional Neural Network (CNN)
to classify nine types of skin cancer from images, potentially reducing diagnosis time and
improving patient outcomes.
# Problem Statement
The current biopsy and analysis process is cumbersome and time-consuming, often taking
over a week from the dermatologist’s initial appointment to the final biopsy report. This
project aims to significantly reduce this timeline to just a few days by employing a predictive
model that classifies various skin cancers using CNN, thereby impacting millions potentially
at risk.
# Motivation
The primary motivation behind this project is to reduce mortality from skin cancer by
employing state-of-the-art image classification technology. Advances in computer vision and
machine learning offer promising tools to improve diagnostic processes and patient care.
# Dataset
The dataset consists of 2,357 dermatoscopic images from the International Skin Imaging
Collaboration (ISIC). These images represent various malignant and benign conditions and
are balanced across different classifications to address potential class imbalances. The
dataset includes augmentation via the Augmentor Python package to ensure no class is
underrepresented.
<img width="398" alt="image" src="https://github.com/user-attachments/assets/ed8a363b-9e16-4200-be96-a523420376b1" />
<img width="208" alt="image" src="https://github.com/user-attachments/assets/ac7a3bdc-4d05-43f7-81b8-c279f0d9c711" />

# CNN Architecture Overview
The proposed CNN architecture for this project is designed to optimize accuracy and
efficiency in skin cancer classification:
1. Rescaling Layer: Normalizes input images from a [0, 255] range to [0, 1] to facilitate
model processing.
2. Convolutional Layers: These layers apply convolution operations to condense
information from the image pixels into feature maps, enhancing feature detection.
3. Pooling Layers: Reduce the dimensionality of each feature map, decreasing the
computational load and the model's sensitivity to the location of features.
4. Dropout Layers: Randomly drops units (with a rate of 50%) from the feature maps to
prevent overfitting.
5. Flatten Layer: Converts the 3D feature maps into 1D feature vectors, preparing data
for the final classification stage.
6. Dense Layers: Fully connected layers that integrate signals from the feature vectors
into predictions for each class.
7. Activation Functions:
o ReLU: Used in hidden layers to introduce non-linearity, helping the model
learn complex patterns.
o Softmax: Used in the output layer to convert logits to probabilities for each
class, ensuring the output sums to one.
Expected Impact
By reducing the diagnostic timeline and enhancing accuracy, this project has the potential to
significantly impact public health. Faster and more reliable diagnostics can lead to earlier
interventions, which are crucial for increasing survival rates in melanoma cases.
Conclusion
This project represents a significant step forward in the application of advanced machine
learning techniques to critical healthcare challenges. By integrating a sophisticated CNN
model with a comprehensive dataset of skin lesion images, we aim to provide a more
efficient and accurate diagnostic tool for melanoma, potentially saving lives through earlier
detection and treatment.
