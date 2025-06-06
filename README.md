# Football-Analytics-with-Computer-Vision

This repository provides a complete workflow for detecting keypoints on images and applying those detections to estimate homography matrices for pitch images.

---

## Project Description

The core of this project is a keypoint detection model trained on annotated images. The trained model is then used to detect relevant keypoints on pitch images, enabling the calculation of the homography matrix. This matrix allows for perspective transformations and spatial mapping on pitch surfaces.

---

## Repository Contents

- **Keypoint Detection Model Training:**  
  Notebook for includes data loading, preprocessing, and training a deep learning model to detect keypoints on images. The dataset consists of images paired with keypoint annotations stored in text (TXT) files.

- **Pitch Keypoint Detection and Homography Estimation:**  
  Notebook to apply the trained model on pitch images to detect keypoints. These detected points are matched to reference points to compute the homography matrix. This transformation can be used for tasks such as image rectification and spatial analysis of pitch layouts.
  
- **dataset:**
  Contains the training, testing and validation images and their corresponding annotations in `.txt` format.
  
 - **models:**
   Directory containing trained model weights for inference or fine-tuning.  


---

## Dataset

- Images with annotated keypoints used for supervised model training.  
- Pitch images with distinguishable landmarks for homography calculation.

Annotations are provided in text (TXT) files specifying keypoint coordinates.

---

## How to Use

1. Prepare the dataset with images and corresponding keypoint annotations in TXT files.  
2. Train the keypoint detection model on the labeled images.  
3. Apply the trained model to pitch images to extract keypoints.  
4. Calculate the homography matrix using matched keypoints to perform perspective transformations.

---

## Dependencies

- Python 3.7+  
- Deep learning framework (PyTorch or TensorFlow)  
- OpenCV  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Jupyter Notebook
