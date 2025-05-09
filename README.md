# Traffic Sign Detection and Classification

A deep learning model for detecting and classifying traffic signs using Convolutional Neural Networks (CNN).

## Overview

This project uses a CNN model to classify traffic signs from images. The model is trained on a dataset of traffic sign images categorized into multiple classes. It can be used for automated traffic sign recognition in self-driving cars, driver assistance systems, or traffic management applications.

## Features

- Image preprocessing with grayscale conversion and histogram equalization
- Data augmentation using ImageDataGenerator
- Convolutional Neural Network architecture with:
  - Multiple convolutional layers
  - MaxPooling layers
  - Dropout for regularization
  - Dense layers for classification
- Training with validation and test split
- Performance visualization (accuracy and loss plots)
- Inference on new images

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/tusharrrrrp/Traffic_sign_detection.git
   cd Traffic_sign_detection
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

## Dataset Structure

The dataset should be organized as follows:
```
Dataset/
├── 0/
│   ├── image1.png
│   ├── image2.png
│   └── ...
├── 1/
│   ├── image1.png
│   └── ...
└── ...
```

Where each numbered folder represents a different traffic sign class.

## Usage

### Training the Model

```python
# The main script contains all necessary code for:
# - Loading and preprocessing data
# - Building the CNN model
# - Training the model
# - Evaluating performance
python train_model.py
```

### Making Predictions

```python
# Example code for using the trained model to make predictions on new images
python predict.py --image path/to/your/image.png
```

## Model Architecture

The CNN architecture consists of:
- Input layer (32x32x1 - grayscale images)
- 2 Convolutional layers with 60 filters (5x5)
- MaxPooling layer
- 2 Convolutional layers with 30 filters (3x3)
- MaxPooling layer
- Dropout layer (50%)
- Flatten layer
- Dense layer (500 neurons)
- Dropout layer (50%)
- Output layer (number of classes)

## Performance

The model achieves:

- Test accuracy: [96%]

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- contact **[shaktiyakshama@gmail.com]** for the dataset and the Label.csv
