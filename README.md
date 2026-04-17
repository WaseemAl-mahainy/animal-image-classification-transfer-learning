#  Animal Image Classification with EfficientNetB0 Transfer Learning

A solo deep learning project that applies transfer learning and fine-tuning using EfficientNetB0 for classifying 10 animal categories from the Animals-10 dataset with TensorFlow/Keras.

## Project Overview

This project focuses on multi-class animal image classification using a pretrained EfficientNetB0 backbone. Instead of training a convolutional neural network entirely from scratch, transfer learning was used to leverage pretrained visual features and then fine-tune the model for stronger performance on the Animals-10 dataset.

The model classifies images into 10 animal categories:
- butterfly
- cat
- chicken
- cow
- dog
- elephant
- horse
- sheep
- spider
- squirrel

## Dataset

- **Dataset:** Animals-10
- **Task:** Multi-class image classification

## Tech Stack

- Python
- TensorFlow / Keras
- EfficientNetB0
- NumPy
- Matplotlib
- scikit-learn
- Jupyter Notebook

## Methodology

This project includes:
- image preprocessing with EfficientNet-specific preprocessing
- data augmentation for training robustness
- transfer learning with EfficientNetB0
- fine-tuning experiments across multiple training stages
- model checkpointing and best-model saving
- evaluation using test accuracy, confusion matrix, and classification report

## Training Strategy

Several fine-tuning experiments were conducted to improve performance, using:
- `ModelCheckpoint`
- `EarlyStopping`
- `ReduceLROnPlateau`

The project compared multiple experiment stages and selected the best-performing model for final evaluation.

## Results

The best selected model achieved approximately:

- **Test Accuracy:** around 93%
- strong overall class-wise precision, recall, and F1-score
- improved performance compared with the from-scratch CNN version

Additional evaluation included:
- confusion matrix
- classification report
- class-wise prediction analysis

## Files in This Repository

- `transfer_learning_animal_classifier.ipynb` — full notebook for transfer learning, fine-tuning, and evaluation
- `requirements.txt` — Python dependencies
- `sample_outputs/` — optional screenshots of training curves and confusion matrix
- `test_images/` — optional small demo images

## How to Run

1. Clone the repository
2. Install dependencies from `requirements.txt`
3. Download the Animals-10 dataset
4. Update dataset paths in the notebook
5. Open and run the notebook step by step

## Future Improvements

- compare EfficientNetB0 with other pretrained backbones
- export the model into an inference-ready application
- add deployment through a simple API or web interface
- test more controlled fine-tuning strategies

## Author

**Waseem Al-Mahainy**  
AI / Machine Learning student engineer
