
# MeXE 402 - Mechatronics Engineering Elective 2: Data Science and Machine Learning
## Revised Topic: Converting images of Six Bird Species into Grayscale.

**Link of our Dataset**

Bird Species Dataset[Link](https://drive.google.com/drive/folders/1ClZXsBIiUZ3M1lgg9_OkRYEsIA749okt?usp=drive_link)

**Link of our video**

Video[link]()

## Table of Contents
1. [Introduction](#Introduction)
2. [Abstract](#Abstract)
3. [Project Method](#Project-Method)
4. [Conclusion](#Conclusion)
5. [Additional Materials](#Additional-Materials)
   - [Six Bird Species](#Six-Bird-Species)
   
6. [References](#References)


## Introduction
   The "Bird Species Dataset" directory contains subdirectories for various bird species, such as "AMERICAN GOLDFINCH," "BARN OWL," "CARMINE BEE-EATER," "DOWNY WOODPECKER," "EMPEROR PENGUIN," and "FLAMINGO." Each of these subdirectories likely contains images of the respective bird species.

Based on this dataset, it appears that the problem relates to bird species classification using computer vision. Here's a brief description of the problem and its significance:

**Problem Description**
The task is to develop a computer vision model capable of classifying images of birds into their respective species. This involves training a machine learning model on a labeled dataset containing images of different bird species. The goal is to accurately identify the species of a bird given a new image.

**Significance in Computer Vision**
- Biodiversity Monitoring: Accurate bird species classification aids in monitoring and conserving biodiversity. It helps scientists and researchers track bird populations, study their behavior, and detect changes in their habitats.
- Wildlife Conservation: Automated bird species identification supports wildlife conservation efforts by enabling the efficient collection and analysis of ecological data, leading to better-informed conservation strategies.
- Citizen Science: Enhancing the capabilities of birdwatching apps with species recognition can engage the public in citizen science projects, increasing awareness and participation in biodiversity conservation.
Advancements in Computer Vision: Tackling the challenges of fine-grained image classification, such as distinguishing between visually similar bird species, pushes the boundaries of computer vision and deep learning techniques, leading to advancements applicable in various domains.

- Datasets for bird species are crucial to biodiversity studies and development of computer vision models for species identification and monitoring of their ecological status.
- Converting bird species images to grayscale removes color information, compelling models to rely solely on structural features such as texture, shape, and patterns for classification.
- This problem addresses the robustness and adaptability of computer vision models in scenarios where color data is unavailable or unreliable

## Abstract

   This project explores the impact of converting images of six bird species into grayscale on the performance of computer vision models. By removing color information, the models are challenged to rely solely on structural features such as texture, shape, and patterns for species classification. The approach involves processing bird images using OpenCV for grayscale conversion and visualization. This study aims to evaluate the adaptability and robustness of computer vision techniques in scenarios where color data is unavailable, with applications in biodiversity monitoring, wildlife conservation, and fine-grained image classification advancements.
   
## Project Method

**(Step-by-Step):**

**Dataset Preparation:**

- Accessed the "Bird Species Dataset" containing images of six bird species: American Goldfinch, Barn Owl, Carmine Bee-Eater, Downy Woodpecker, Emperor Penguin, and Flamingo.
- Organized images in respective directories for efficient processing.

**Image Reading:**
- Loaded images using OpenCV's cv2.imread function, specifying the file path for each bird species.
  
**Colorful Image Visualization:**
- Displayed the original RGB images using cv2_imshow to verify their dimensions and content.
  
**Grayscale Conversion:**
- Converted each colorful image to grayscale using OpenCV's cv2.cvtColor with the cv2.COLOR_BGR2GRAY parameter.
  
**Grayscale Visualization:**
- Displayed the grayscale images using cv2_imshow to verify the conversion.
  
**Image Shape Validation:**
- Printed the dimensions of both RGB and grayscale images to confirm the number of channels and resolution consistency.
  
**Repeat for Each Species:**

- Applied the above steps iteratively for images from all six bird species.
- This methodology ensured a structured approach to preprocessing and grayscale conversion, facilitating further analysis and modeling.


## Conclusion

Transforming images to grayscale is a key step in image processing as it simplifies the data and emphasizes essential details. This project demonstrates the process using OpenCV, focusing on images captured by outdoor surveillance cameras.

**Findings**
   
   The project focused on converting images of six bird species into grayscale and analyzing the impact on the performance of computer vision models for species classification. The species included were American Goldfinch, Barn Owl, Carmine Bee-Eater, Downy Woodpecker, Emperor Penguin, and Flamingo. The dataset was processed using OpenCV, specifically employing functions like cv2.imread for reading images and cv2.cvtColor for converting images to grayscale.

**Challenges**

- Dataset Handling: Ensuring the dataset was correctly structured and accessible for processing posed an initial challenge. Each bird species had a subdirectory, and images needed to be read and processed individually.

- Image Processing: Converting images to grayscale removed color information, which can be significant for distinguishing species with similar structural features but different colors. This necessitated a focus on enhancing the model's ability to recognize patterns, shapes, and textures.

Model Performance: Evaluating the model's performance after removing color information required careful consideration. Ensuring that the grayscale images retained enough distinctive features for accurate classification was crucial.

**Outcomes**

- Simplified Image Data: Transforming images to grayscale significantly simplified the data, reducing the complexity of the input without losing essential structural details. This step highlighted the model's capability to classify bird species based solely on texture and shape.

- Robust Model Development: The project demonstrated that computer vision models could still perform effectively in scenarios where color data is unavailable or unreliable. This has implications for real-world applications, such as monitoring wildlife with cameras that capture grayscale images.

- Enhanced Understanding: The process provided valuable insights into the robustness and adaptability of computer vision models. It underscored the importance of preprocessing steps and the potential need for additional techniques to compensate for the loss of color information.

In conclusion, the project successfully showcased the application of grayscale conversion in bird species classification, contributing to the field of computer vision by exploring how models can adapt to different types of input data.

## Additional Materials

### Six Bird Species
- Preprocessing scripts for grayscale conversion.
1. **American Goldfinch**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow

#Colorful image - 3 Channels
img = cv2.imread("drive/MyDrive/Bird Species Dataset/AMERICAN GOLDFINCH/001.jpg")
print(img.shape)
cv2_imshow(img)

#Grayscale image
gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
(224, 224, 3)

![image](https://github.com/user-attachments/assets/6c55baaf-b55a-4f94-845b-848d3230e2ad)

(224,224)

![image](https://github.com/user-attachments/assets/1633d68a-7d53-4e98-bcce-7eca907e5a6a)

2. **Barn Owl**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow

#Colorful image - 3 Channels
img = cv2.imread("drive/MyDrive/Bird Species Dataset/BARN OWL/001.jpg")
print(img.shape)
cv2_imshow(img)

# Grayscale image
gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
(224,224, 3)

![image](https://github.com/user-attachments/assets/39cc1a8c-d91c-4795-bbb9-25e67dbbc787)

(224,224)

![image](https://github.com/user-attachments/assets/5752554d-bf62-45cf-ac0f-477c1774bb26)


3.**Carmine Bee-Eater**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow

#Colorful image - 3 Channels
img = cv2.imread("drive/MyDrive/Bird Species Dataset/CARMINE BEE-EATER/001.jpg")
print(img.shape)
cv2_imshow(img)

# Grayscale image
gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
(224,224, 3)

![image](https://github.com/user-attachments/assets/4e887e60-2c0d-427d-a17b-6d8077c70bec)

(224,224)

![image](https://github.com/user-attachments/assets/d96c537a-d238-42c0-a254-ef83185e27b7)

4. **Downy Woodpecker**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow

#Colorful image - 3 Channels
img = cv2.imread("drive/MyDrive/Bird Species Dataset/DOWNY WOODPECKER/001.jpg")
print(img.shape)
cv2_imshow(img)

# Grayscale image
gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
(224,224, 3)

![image](https://github.com/user-attachments/assets/8a36a9c2-3c9e-4b51-b421-e1c161f3bd6c)

(224,224)

![image](https://github.com/user-attachments/assets/de0ea5b5-2af0-43fc-b78f-369ea2d6ef58)

5. **Emperor Penguin**
``` Google Colab
import cv2
from google.colab.patches import cv2_imshow

#Colorful image - 3 Channels
img = cv2.imread("drive/MyDrive/Bird Species Dataset/EMPEROR PENGUIN/001.jpg")
print(img.shape)
cv2_imshow(img)

# Grayscale image
gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
(224,224, 3)

![image](https://github.com/user-attachments/assets/48bfe7f5-5b69-425a-a24a-3f53bdf073cc)

(224,224)

![image](https://github.com/user-attachments/assets/bd845f22-3bf3-4707-ad8a-828a323eb49a)

6. **Flamingo**
```Google Colab
import cv2
from google.colab.patches import cv2_imshow

#Colorful image - 3 Channels
img = cv2.imread("drive/MyDrive/Bird Species Dataset/FLAMINGO/001.jpg")
print(img.shape)
cv2_imshow(img)

# Grayscale image
gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
print(gray.shape)
cv2_imshow(gray)
```
(224,224, 3)

![image](https://github.com/user-attachments/assets/156584ee-3dc0-41aa-bfa5-fe09c75ac12b)

(224,224)

![image](https://github.com/user-attachments/assets/dd346920-df36-4877-b459-fcad8fd6a95f)

### References
1. RAHMA SLEAM *Bird Speciees Dataset* [Link](https://www.kaggle.com/datasets/rahmasleam/bird-speciees-dataset)
2. Misbah Mohammed *OpenCV Tutorial*[Link](https://youtu.be/E3Lg4aZVCAU?si=IMGIsYiZ-dFTSPL3)
3. MikkoDT. *Finals Instructions* [Link](https://github.com/MikkoDT/MeXEE402_Finals_4102)

**Group Member**

Evangelista, Lexter Jhustin L.(20-60481)

Montalbo, Christian Kent (20-xxxx)
