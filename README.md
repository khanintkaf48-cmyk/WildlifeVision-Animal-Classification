# WildlifeVision – Animal Image Classifier

WildlifeVision is an image-classification project that uses deep learning to identify animals from images. The notebook explores a 10-category subset of the Animal-10 dataset and compares two transfer-learning architectures: **VGG16** and **ResNet50**.

## Project Overview

The notebook demonstrates an end-to-end image-classification workflow:

- Load and explore the Animal-10 image dataset.
- Prepare and resize images to 224 × 224 pixels.
- Shuffle the data and create training and validation sets.
- Normalize image pixel values and apply data augmentation.
- Build and train VGG16- and ResNet50-based models.
- Compare training/validation accuracy and loss.
- Predict animal categories for sample test images.

## Animal Categories

The dataset contains these 10 categories:

- Butterfly
- Cat
- Chicken
- Cow
- Dog
- Elephant
- Horse
- Sheep
- Spider
- Squirrel

## Models

The notebook experiments with:

- **VGG16** – an ImageNet-pretrained convolutional neural network used as a feature extractor.
- **ResNet50** – a 50-layer residual network.

The notebook records the following validation results:

| Model | Recorded validation accuracy |
|---|---:|
| VGG16 | 96.21% |
| ResNet50 | 90.17% |

These are the results recorded in the supplied notebook; results may vary when the notebook is rerun with different environments, data splits, or training settings.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- OpenCV
- Matplotlib
- scikit-learn
- tqdm
- Jupyter Notebook

## Dataset

The project uses the **Animal-10** dataset.

Dataset source: [Animal-10 on Kaggle](https://www.kaggle.com/datasets/alessiocorrado99/animals10)

Download the dataset from Kaggle and make sure its extracted directory is available at the path expected by the notebook:

```text
/kaggle/input/animals10/raw-img
```

The notebook was written for a Kaggle-style environment. If you run it locally or in another notebook environment, update the dataset paths to match your machine.

## How to Run

1. Clone or download this repository.
2. Download and extract the Animal-10 dataset from Kaggle.
3. Open `wildlife_animal_classifier.ipynb` in Jupyter Notebook, JupyterLab, or Kaggle.
4. Confirm that the dataset path in the notebook points to the extracted `raw-img` folder.
5. Run the notebook cells in order.

Install the main Python packages if they are not already available:

```bash
pip install numpy pandas matplotlib tensorflow opencv-python scikit-learn tqdm
```

> Note: TensorFlow/Keras APIs can differ between versions. The notebook uses some older Keras training and optimizer arguments, so a compatible environment may be required to run it without code updates.

## Repository Structure

```text
WildlifeVision-Animal-Image-Classifier/
├── README.md
└── wildlife_animal_classifier.ipynb
```

## Project Scope

This repository contains the supplied Jupyter notebook and its documentation. The dataset and trained model-weight files are not included in this ZIP; download the dataset separately using the link above.

## License

No license file was included with the supplied project. Add a license only after confirming the licensing terms for your code and the dataset.
