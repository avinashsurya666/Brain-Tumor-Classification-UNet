# Brain Tumor Classification Using U-Net Image Segmentation and Classification

## Project Description

This project focuses on brain tumor classification through a two-stage process involving image segmentation and classification. The U-Net model is used for segmenting tumor regions in brain MRI scans. Once segmented, a classification model identifies the tumor type (e.g., glioma, meningioma, or pituitary tumor) based on the segmented regions.

By combining U-Net for segmentation and a classification model, this pipeline improves the accuracy and efficiency of brain tumor diagnosis, which can aid medical professionals in treatment planning.

---

## Features

- **U-Net Image Segmentation**: U-Net is utilized to accurately segment brain tumors from MRI images.
- **Classification**: After segmentation, the tumor region is classified to determine the type of tumor.
- **Medical Dataset**: Trained and tested on a publicly available brain MRI dataset.
- **End-to-End Pipeline**: Provides a complete workflow from segmentation to classification.

---

## Getting Started

### Prerequisites

- Python 3.8+
- TensorFlow or PyTorch
- OpenCV
- NumPy, Matplotlib, and other Python libraries
- A medical brain MRI dataset (e.g., Kaggle, TCIA)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/brain-tumor-classification.git
    cd brain-tumor-classification
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Download the brain MRI dataset:
    - Download a brain MRI dataset and place it in the `./data/brain_tumor/` directory.

---

## Training the Model

### Train U-Net for Segmentation

To train the U-Net model for tumor segmentation:

```bash
python train_unet.py --dataset ./data/brain_tumor/
