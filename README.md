# Documentation for ML_PadiCare Project

## Project Description
The **ML_PadiCare** project is a machine learning model designed to classify types of diseases in rice plants using MobileNetV2. The dataset includes four categories: **Hispa**, **Leaf Blast**, **Brown Spot**, and **Healthy**. Additionally, the project features model conversion to TensorFlow Lite (TFLite) format for deployment on resource-constrained devices.

---

## Repository Structure
1. **Dataset**
   - The dataset is divided into two parts:
     - **Train**: Data used for training the model.
     - **Validation**: Data used for evaluating the model's performance.
   - Categories in the dataset:
     - **Hispa**: Images of rice leaves affected by hispa.
     - **Leaf Blast**: Images of rice leaves affected by leaf blast.
     - **Brown Spot**: Images of rice leaves affected by brown spot.
     - **Healthy**: Images of healthy rice leaves.

2. **Model Code**
   - **MobileNetV2** is used as the architecture for image classification.
   - The code includes:
     - Data preprocessing (augmentation, normalization, and data splitting).
     - Model training using the provided dataset.
     - Model evaluation on the validation dataset.

3. **TFLite Conversion**
   - After training, the model is converted to TensorFlow Lite (TFLite) format.
   - The TFLite format enables model usage on edge devices such as mobile phones or IoT devices.

---

## Usage Guide

### 1. Prerequisites
- Python 3.7 or higher
- TensorFlow
- NumPy
- Matplotlib

### 2. Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/ArPaWi/ML_PadiCare.git
   cd ML_PadiCare
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### 3. Training the Model
1. Ensure the dataset is structured into `train` and `validation` folders.
2. Run the training script:
   ```bash
   python dev_padicare.ipynb
   ```
   - The trained model will be saved in the `models/` folder.

### 4. Converting the Model to TFLite
1. After run the code The TFLite model will be saved in the `tflite_models/` folder.

### 5. Converted Model
1. The converted model can be accessed in the `models/` `tflite/` folder in this repository.

## Penulis

Proyek ini dikembangkan oleh:

- Arya Panca Wibowo
- Delima Ester Purba
- Muhammad Rafli Ardiansyah
