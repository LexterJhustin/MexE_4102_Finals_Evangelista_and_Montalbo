# Final Project in Electives 2
## Revised Topic: Converting images of Six Bird Species into Grayscale.

## Table of Contents
1. [Introduction](#Introduction)
2. [Abstract](#Abstract)
3. [Project Method](#Project-Method)
4. [Conclusion](#Conclusion)
5. [Additional Materials](#Additional-Materials)


## Introduction
- Datasets for bird species are crucial to biodiversity studies and development of computer vision models for species identification and monitoring of their ecological status.
- Converting bird species images to grayscale removes color information, compelling models to rely solely on structural features such as texture, shape, and patterns for classification.
- This problem addresses the robustness and adaptability of computer vision models in scenarios where color data is unavailable or unreliable

## Abstract
This project investigates the impact of converting bird species images to grayscale on the performance of computer vision models.

## Project Method

## Conclusion

## Additional Materials

### Six Bird Species
1. **American Goldfinch**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow
img = cv2.imread("drive/MyDrive/Bird Species Dataset/AMERICAN GOLDFINCH/001.jpg")
#img = cv2.resize(img,(500,500))
print(img.shape)
cv2_imshow(img)

gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
2. **Barn Owl**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow
img = cv2.imread("drive/MyDrive/Bird Species Dataset/BARN OWL/001.jpg")
#img = cv2.resize(img,(500,500))
print(img.shape)
cv2_imshow(img)

gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
