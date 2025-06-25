# SmartCassava
An AI Powered-Mobile Solution for Cassava Leaf Diagnosis, Severity Analysis, and Farmer Support.

## Features

- Image-based cassava disease classification
- Five-class prediction:
  - Cassava Mosaic Disease (CMD)
  - Cassava Bacterial Blight (CBB)
  - Cassava Brown Streak Disease (CBSD)
  - Cassava Green Mite (CGM)
  - Healthy
- Integrated data augmentation for better generalization
- Training done using EfficientNetB0 and TensorFlow
- Deployable via TensorFlow Lite for mobile apps

## Dataset

- Source: [Kaggle Cassava Leaf Disease Classification](https://www.kaggle.com/competitions/cassava-leaf-disease-classification/data)
- Includes:
  - `train/` folder with images
  - `train.csv` file with image filenames and numeric labels

## How to Train (Colab)
1. Open [`cassava_training.ipynb`](notebooks/cassava_training.ipynb) in Google Colab
2. Mount your Google Drive
3. Upload your dataset (`train/` and `train.csv`)
4. Run all cells — training, evaluation, and export

## Label Map

```python
label_map = {
    0: "Cassava Bacterial Blight (CBB)",
    1: "Cassava Brown Streak Disease (CBSD)",
    2: "Cassava Green Mottle (CGM)",
    3: "Cassava Mosaic Disease (CMD)",
    4: "Healthy"
}
