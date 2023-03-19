# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: Vismaya.S 
### Register Number: 212221230125
i) #To Read,display the image
```
import cv2
import matplotlib.pyplot as plt
from google.colab.patches import cv2_imshow
color_image = cv2.imread('T.jpg',1)
cv2_imshow(color_image)  

```
ii) #To write the image
```
color_image = cv2.imread('T.jpg',1)
cv2_imshow(color_image)
cv2.imwrite('212221230125VISMAYA.jpg',color_image)



```
iii) #Find the shape of the Image
```python3

import cv2
color=cv2.imread('T.jpg',1)
print(color.shape)




```
iv) #To access rows and columns

```python3

import cv2
import random
color_image= cv2.imread('T.jpg',1)
for i in range(150):
    for j in range(color_image.shape[1]):
        color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2_imshow(color_image)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```python3

import cv2
color_imagw= cv2.imread('T.jpg',-1)
new = color_image[300:450,300:450]
color_image[250:400,250:400] = new
cv2_imshow(color_image)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image

<br>![output](o1.png)
<br>

### ii)Write the image

<br>![output](o2.png)
<br>

### iii)Shape of the Image

<br>![output](o3.png)
<br>

### iv)Access rows and columns
<br>![output](o4.png)
<br>

### v)Cut and paste portion of image
<br> ![output](o5.png)
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


