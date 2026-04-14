# Plant Disease Classification using Hybrid Transfer Learning

## Overview

This project presents a hybrid transfer learning framework for plant disease classification using lightweight deep learning models. The approach is designed for resource-constrained environments such as edge AI systems and agricultural IoT applications.

The framework uses a two-stage training strategy:

* Stage 1: Domain-adaptive pretraining on the PlantVillage dataset
* Stage 2: Fine-tuning on the PlantDoc dataset

## Models

* EfficientNetV2B0
* MobileNetV3Small

## Datasets

### PlantVillage (Source Domain)

https://drive.google.com/drive/folders/1WLxetk2DPIO41wjkbEpVPOG4Omn1ir1p

### PlantDoc (Target Domain)

https://drive.google.com/drive/folders/1Izt0FxV3TUkgz7QMREkxDCBnxEDh4Do8

## Code

The implementation is available both as a Google Colab notebook and as a downloadable Jupyter Notebook file:

* Google Colab:
  https://colab.research.google.com/drive/1CsnXWigaiYHl2uKf76vMZUvwPRwYGvyZ

* GitHub (.ipynb file):
  `notebooks/hybrid_transfer_learning.ipynb`

The notebook can be directly executed in Google Colab without additional setup. For local execution, the `.ipynb` file can be downloaded from this repository.
## DOI

https://doi.org/10.5281/zenodo.19564312

## Requirements

* Python 3.x
* TensorFlow / Keras
* NumPy
* Pandas
* Matplotlib
* scikit-learn

## Usage

1. Download datasets from the links above
2. Upload datasets to Google Drive
3. Open the Colab notebook
4. Update dataset paths if necessary
5. Run all cells

## Methodology

* Transfer learning with ImageNet weights
* Hybrid transfer learning (PV → PD)
* Evaluation using both classification and resource-efficiency metrics

## Evaluation Metrics

* Accuracy
* Precision, Recall, F1-score
* Micro-AUC
* GFLOPs
* Latency

## Ablation Study

* No-Pretrain (ImageNet only)
* Hybrid Transfer Learning (PV → PD)

## Reproducibility

All experiments were conducted in Google Colab with GPU support. Training configurations and dataset splits are described in the manuscript.

## License

This project is licensed under the MIT License.

## Dataset License

The datasets (PlantVillage and PlantDoc) are publicly available and subject to their respective licenses and usage terms.
