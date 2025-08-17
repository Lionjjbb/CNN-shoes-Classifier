# Shoe Brand Classification Model

## Overview
This project uses a TensorFlow/Keras CNN to classify shoe images into Adidas, Converse, and Nike categories. The `training_script.ipynb` notebook handles data preprocessing, model loading, and evaluation.

## Prerequisites
- Python 3.x
- TensorFlow, matplotlib, numpy, pillow
- Google Colab with GPU (optional)
- Google Drive dataset with `train`, `validate`, and `new_test_sub` folders, each containing `adidas`, `converse`, `nike` subdirectories

## Installation
1. Open `training_script.ipynb` in Google Colab.
2. Install dependencies:
   ```bash
   pip install tensorflow matplotlib numpy pillow
   ```
3. Mount Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/gdrive')
   ```

## Dataset
- **Path**: `/content/gdrive/MyDrive/`
- **Structure**: Subdirectories `train`, `validate`, `new_test_sub` with class folders
- **Image size**: 240x240 pixels
- **Batch size**: 32

## Usage
1. Run `training_script.ipynb` in Colab.
2. Loads `Mymodel2.keras` and evaluates on test dataset.
3. Outputs test accuracy, loss, and sample count.

## Model
- CNN with Conv2D, MaxPooling, Dropout, Dense layers
- Optimizer: Adam
- Loss: Sparse Categorical Crossentropy
- Metric: Accuracy

## Notes
- Update dataset paths if different.
- Uncomment augmentation/model definition for training.
- Low accuracy (33.33%) may require more epochs or data.

## GitHub
1. Clone: `git clone https://github.com/your-username/shoe-classification-model.git`
2. Add `training_script.ipynb`, `README.md` to repo.
3. Push: `git add . && git commit -m "Initial commit" && git push origin main`