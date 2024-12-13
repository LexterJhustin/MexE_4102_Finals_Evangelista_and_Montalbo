# Final Project in Electives 2
## Revised Topic: Converting images of Six Bird Species into Grayscale.

## Table of Contents
1. [Introduction](#Introduction)
2. [Abstract](#Abstract)
3. [Project Method](#Project-Method)
4. [Conclusion](#Conclusion)
5. [Additional Materials](#Additional-Materials)
   - [Six Bird Species](#Six-Bird-Species)
      1. [American Goldfinch](####**American-Goldfinch**)
      2. [Barn Owl](#**Barn-Owl**)
      3. [Carmine Bee-Eater](#**Carmine-Bee-Eater**)
      4. [Downy Woodpecker](#**Downy-Woodpecker**)
      5. [Emperor Penguin](#**Emperor-Penguin**)
      6. [Flamingo](#**Flamingo**)
6. [References](#References)


## Introduction
- Datasets for bird species are crucial to biodiversity studies and development of computer vision models for species identification and monitoring of their ecological status.
- Converting bird species images to grayscale removes color information, compelling models to rely solely on structural features such as texture, shape, and patterns for classification.
- This problem addresses the robustness and adaptability of computer vision models in scenarios where color data is unavailable or unreliable

## Abstract
This project investigates the impact of converting bird species images to grayscale on the performance of computer vision models.

## Project Method

When working with image datasets like the bird species dataset, cv2 is often used for tasks such as:

- Reading and writing image files (cv2.imread and cv2.imwrite).
- Converting images between color spaces (e.g., RGB to Grayscale with cv2.cvtColor).
- Visualizing images using OpenCV's display functionality (cv2.imshow).
## Conclusion

## Additional Materials

### Six Bird Species
- Preprocessing scripts for grayscale conversion.
#### 1. **American Goldfinch**
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
#### 2. **Barn Owl**
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
#### 3.**Carmine Bee-Eater**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow
img = cv2.imread("drive/MyDrive/Bird Species Dataset/CARMINE BEE-EATER/001.jpg")
#img = cv2.resize(img,(500,500))
print(img.shape)
cv2_imshow(img)

gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
#### 4. **Downy Woodpecker**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow
img = cv2.imread("drive/MyDrive/Bird Species Dataset/DOWNY WOODPECKER/001.jpg")
#img = cv2.resize(img,(500,500))
print(img.shape)
cv2_imshow(img)

gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
#### 5. **Emperor Penguin**
``` Google Colab
import cv2
from google.colab.patches import cv2_imshow
img = cv2.imread("drive/MyDrive/Bird Species Dataset/EMPEROR PENGUIN/001.jpg")
#img = cv2.resize(img,(500,500))
print(img.shape)
cv2_imshow(img)

gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
#### 6. **Flamingo**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow
img = cv2.imread("drive/MyDrive/Bird Species Dataset/FLAMINGO/001.jpg")
#img = cv2.resize(img,(500,500))
print(img.shape)
cv2_imshow(img)

gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
### References
1. RAHMA SLEAM *Bird Speciees Dataset* [Link](https://www.kaggle.com/datasets/rahmasleam/bird-speciees-dataset)
2. Misbah Mohammed *OpenCV Tutorial*[Link](https://youtu.be/E3Lg4aZVCAU?si=IMGIsYiZ-dFTSPL3)
3. MikkoDT. *Finals Instructions* [Link](https://github.com/MikkoDT/MeXEE402_Finals_4102)
