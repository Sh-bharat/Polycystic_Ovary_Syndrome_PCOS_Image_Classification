---

# PCOS Ultrasound Image Dataset

## Overview
This dataset contains ultrasound images for the classification of Polycystic Ovary Syndrome (PCOS). The dataset originally sourced from [PCOS Dataset](https://www.kaggle.com/datasets/shnotweta/2000-images-of-ultrasound-for-pcos) contained noisy images with irregular boundaries. These images were cleaned, cropped, and processed to remove irregularities. The dataset has been split into training and testing sets with a ratio of 80:20.

## Contents
- `train/`: Directory containing cleaned ultrasound images for training.
- `test/`: Directory containing cleaned ultrasound images for testing.

## Usage
Researchers and practitioners can utilize this dataset for the development and evaluation of PCOS classification algorithms using ultrasound images. The cleaned dataset ensures reliable training and testing results.  [Cleaned PCOS Dataset](https://www.kaggle.com/datasets/bharatsh001/pcos-cleaned-and-splitted)

## Datset Information
There are total of  2 Classes.
  *  NORMAL : 1142 Files
  *  PCOS : 844 Files<br><hr>
PCOS UltraSound Images <br> 
<img src="https://github.com/Sh-bharat/PCOS_Image_Classification/assets/133742551/5acad53b-5259-4bc5-8a4d-183e7731d7a0" width="700" height="450" /><br>Normal UltraSound Images <br> <img src="https://github.com/Sh-bharat/PCOS_Image_Classification/assets/133742551/dda76bf0-cfc4-4ff6-b1f3-3294885e3f22" width="700" height="450" />


## Trained YOLO Model
The YOLO (You Only Look Once) model has been trained on the cleaned dataset, achieving the best accuracy for PCOS classification.

- **Model Architecture**: YOLOv8 (You Only Look Once version 8)
- **Accuracy**: 99.9%
- **Training Details**:Epochs=50

## Results
<img src="https://github.com/Sh-bharat/PCOS_Image_Classification/assets/133742551/a8389e1f-8023-4af4-85b0-4f9a098d2875" width="500" height="300" />



## Acknowledgements
Special thanks to the original contributors of the [source dataset](https://www.kaggle.com/datasets/shnotweta/2000-images-of-ultrasound-for-pcos) for making this dataset available.

