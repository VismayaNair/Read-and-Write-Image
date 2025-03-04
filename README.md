
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

![o1](https://user-images.githubusercontent.com/93427210/226157471-1f62b040-6238-4a85-910b-35b1d2cecdd4.png)


### ii)Write the image



![o2](https://user-images.githubusercontent.com/93427210/226157634-f0333b8d-1e64-49f1-8c22-5b0b341709eb.png)

### iii)Shape of the Image


<br>![o3](https://user-images.githubusercontent.com/93427210/226157711-1fd1478b-5a3a-46c8-b52f-d73f6c6bbfcc.png)


### iv)Access rows and columns

<br>!
![o4](https://user-images.githubusercontent.com/93427210/226157940-1e830154-3bde-46c4-8824-fe7c532490a5.png)

### v)Cut and paste portion of image

<br>

![o5](https://user-images.githubusercontent.com/93427210/226158182-fab6ee7f-3b12-4c1e-a10f-1f83d7f3b337.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.





