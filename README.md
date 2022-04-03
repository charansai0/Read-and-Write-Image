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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('c.png',1)
cv2.imshow('21221240061,V.Charan sai',color_img)
cv2.waitKey(0)
  

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('c.png',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('21221240061,V.Charan sai',color_img)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```python3
import cv2
colorImage = cv2.imread('c.png',1)
print(colorImage.shape)


```
iv) #To access rows and columns

```python3
import cv2
import random
color_img=cv2.imread('c.png',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('21221240061,V.Charan sai',color_img)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```python3
import cv2
color_img = cv2.imread('c.png',1)
tag = color_img[20:80,20:80]
color_img[90:150,90:150] = tag
cv2.imshow('21221240061,V.Charan sai',color_img)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image

![output](https://github.com/charansai0/Read-and-Write-Image/blob/main/c1.JPG?raw=true)

### ii)Write the image

![output](https://github.com/charansai0/Read-and-Write-Image/blob/main/c2.JPG?raw=true)

### iii)Shape of the Image

![output](https://github.com/charansai0/Read-and-Write-Image/blob/main/c3.JPG?raw=true)


### iv)Access rows and columns
![output](https://github.com/charansai0/Read-and-Write-Image/blob/main/c4.JPG?raw=true)


### v)Cut and paste portion of image
![output](https://github.com/charansai0/Read-and-Write-Image/blob/main/c5.JPG?raw=true)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


