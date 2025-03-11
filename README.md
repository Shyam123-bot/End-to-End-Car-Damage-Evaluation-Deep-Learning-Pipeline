# End-to-End-Car-Damage-Evaluation-Deep-Learning-Pipeline
An end-to-end deep learning pipeline for vehicle damage detection and severity assessment using computer vision. This project leverages TensorFlow, Keras, Flask, and Bootstrap to classify vehicle damage, identify affected areas, and assess severity. Implemented a multi-stage Convolutional Neural Network (CNN) model for classification. 

## Overview

The project is divided into four main pipelines:
1. **Pipe1**: Verifies if the input image contains a car.
2. **Pipe2**: Detects whether the car in the image is damaged.
3. **Pipe3**: Classifies the location of the damage (front, rear, or side).
4. **Pipe4**: Assesses the severity of the damage (minor, moderate, or severe).

The pipelines use pre-trained deep learning models (e.g., VGG16, ResNet50) and fine-tuned models to achieve high accuracy in their respective tasks.

---

## Pipelines

### Pipe1: Car Verification
- **Objective**: Ensure the input image contains a car.
- **Model**: VGG16 (fine-tuned on car images).
- **Output**: Confirms if the image is a car or not.

### Pipe2: Damage Detection
- **Objective**: Detect if the car in the image is damaged.
- **Model**: Fine-tuned binary classification model.
- **Output**: Indicates whether the car is damaged or not.

### Pipe3: Damage Location Classification
- **Objective**: Classify the location of the damage (front, rear, or side).
- **Model**: Fine-tuned multi-class classification model.
- **Output**: Returns the predicted location of the damage.

### Pipe4: Damage Severity Assessment
- **Objective**: Assess the severity of the damage (minor, moderate, or severe).
- **Model**: Fine-tuned multi-class classification model.
- **Output**: Returns the predicted severity of the damage.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/car-damage-assessment.git
   cd car-damage-assessment
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the pre-trained models and place them in the appropriate directories (e.g., `data1`, `data2`, `data3`, `data4`).

---

## Usage

1. Run the Flask application:
   ```bash
   python app.py
   ```

2. Open your browser and navigate to `http://127.0.0.1:5000/`.

3. Upload an image of a car to assess damage.

4. View the results, including:
   - Whether the image contains a car.
   - Whether the car is damaged.
   - The location of the damage (if applicable).
   - The severity of the damage (if applicable).

---

## Dataset

The project uses the following datasets:
- **Car Images**: A dataset of car images (damaged and undamaged).
- **Damage Location**: A dataset of car images labeled with damage locations (front, rear, side).
- **Damage Severity**: A dataset of car images labeled with damage severity (minor, moderate, severe).

The datasets are split into training and validation sets for model training and evaluation.

---

## Models

The following models are used in the project:
- **VGG16**: Pre-trained on ImageNet and fine-tuned for car verification and damage detection.
- **Custom CNN**: Fine-tuned for damage location and severity classification.

---

## Results

The models achieve the following performance:
- **Car Verification**: ~95% accuracy.
- **Damage Detection**: ~90% accuracy.
- **Damage Location Classification**: ~75% accuracy.
- **Damage Severity Assessment**: ~80% accuracy.

---

## Contributing

Contributions are welcome! If you'd like to contribute, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes.
4. Submit a pull request.

