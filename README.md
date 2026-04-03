# Pneumonia Classification

This project builds a deep learning model to classify pneumonia from chest X-ray images.

## Dataset
Dataset is not included due to size limitations.
Download from: https://drive.google.com/drive/folders/1cH19fxwDKxFh3mGrDqetNWUplhPJPIpe?usp=sharing

## Features
- Data preprocessing & augmentation
- Deep learning model (DenseNet121)
- Model evaluation

## Tech Stack
Python, PyTorch, OpenCV

## Data Augmentation

To improve model generalization and robustness, various data augmentation techniques were applied to simulate real-world variations in chest X-ray images. These transformations help the model handle differences in orientation, position, and lighting conditions.

**Techniques used:**
- Rotation
- Shifting
- Zooming
- Brightness adjustment
- Horizontal flipping

  ## Data Preprocessing

Image preprocessing was performed to enhance image quality, standardize input data, and improve feature extraction for model training. Multiple preprocessing pipelines were explored to evaluate their impact on model performance.

### Preprocessing Pipeline 1 (Zero-DCE)
- Applied Zero-DCE for low-light enhancement and contrast improvement

### Preprocessing Pipeline 2
- CLAHE (contrast enhancement)
- Gaussian Blur (noise reduction)
- Resize
- Normalize

### Preprocessing Pipeline 3
- CLAHE
- Sobel Edge Detection
- Unsharp Mask (edge sharpening)

### Preprocessing Pipeline 4
- BGR to RGB conversion
- Center Crop
- Resize
- Normalize


<img width="648" height="285" alt="Screen Shot 2569-04-04 at 00 10 57" src="https://github.com/user-attachments/assets/b55f5dc2-9db9-4b27-8c84-63ccf14d4db0" />
