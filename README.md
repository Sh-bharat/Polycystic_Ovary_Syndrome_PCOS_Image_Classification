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
<img src="https://github.com/Sh-bharat/Polycystic_Ovary_Syndrome_PCOS_Image_Classification/assets/133742551/a023a1a0-ce1d-4402-903d-108c62ceca0f" width="700" height="450" /><br>Normal UltraSound Images <br> <img src="https://github.com/Sh-bharat/Polycystic_Ovary_Syndrome_PCOS_Image_Classification/assets/133742551/635e833c-8b01-42fb-aede-0f152dfd304d" width="700" height="450" />

## CNN Model
```Sequential```
| Layer (type) | Output Shape | Param # |
|--------------|--------------|---------|
| conv2d (Conv2D) | (1, 254, 254, 64) | 1792 |
| max_pooling2d (MaxPooling2D) | (1, 127, 127, 64) | 0 |
| conv2d_1 (Conv2D) | (1, 125, 125, 32) | 18464 |
| max_pooling2d_1 (MaxPooling2D) | (1, 62, 62, 32) | 0 |
| flatten (Flatten) | (1, 123008) | 0 |
| dense (Dense) | (1, 32) | 3936288 |
| dense_1 (Dense) | (1, 1) | 33 |
| **Total params:** | **3,956,577** |
| **Trainable params:** | **3,956,577** |
| **Non-trainable params:** | **0** |

This CNN Model has been trained on the cleaned dataset, achieving the accuracy of 1.0 for PCOS classification in 10 epochs.

## Trained YOLO Model
The YOLO (You Only Look Once) model has been trained on the cleaned dataset, achieving the accuracy for PCOS classification.

- **Model Architecture**: YOLOv8 (You Only Look Once version 8)
- **Accuracy**: 0.9999
- **Training Details**:Epochs=50


## Results
<img src="https://github.com/Sh-bharat/Polycystic_Ovary_Syndrome_PCOS_Image_Classification/assets/133742551/ded51615-8978-422e-8709-1048a95912ea" width="500" height="300" />



## Acknowledgements
Special thanks to the original contributors of the [source dataset](https://www.kaggle.com/datasets/shnotweta/2000-images-of-ultrasound-for-pcos) for making this dataset available.

