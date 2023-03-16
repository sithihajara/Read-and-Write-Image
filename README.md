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
### Developed By:SITHI HAJARA I
### Register Number:212221230102 
i) #To Read,display the image
```
import cv2
color= cv2.imread('mm.png',1)
cv2.imshow('212221230102',color)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
color= cv2.imread('mm.png',-1)
cv2.imwrite('mm.png',color)


```
iii) #Find the shape of the Image
```
import cv2
color=cv2.imread('mm.png',1)
print(color.shape)

```
iv) #To access rows and columns

```
import cv2
import random
img= cv2.imread('mm.png',-1)
for i in range(300):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221230102 SITHI HAJARA',img)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color=cv2.imread('mm.png',-1)
tag=color[200:300,200:300]
color[100:200,100:200]=tag
cv2.imshow('212221230102 SITHI HAJARA',color)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### i) Read and display the image

![im1](https://user-images.githubusercontent.com/94219582/225508792-a1340520-4642-4a40-9eb1-c04a196208fd.png)


### ii)Write the image


![wr](https://user-images.githubusercontent.com/94219582/225509116-47c1c412-43bb-48b4-b55b-d1c9a4e2eeff.png)


### iii)Shape of the Image


![sh](https://user-images.githubusercontent.com/94219582/225509233-e362cf23-22da-4eb2-97bc-4c0fa82ee271.png)

### iv)Access rows and columns

![im2](https://user-images.githubusercontent.com/94219582/225509276-e3f06290-fad7-439f-886e-ebed077c1a28.png)

### v)Cut and paste portion of image

![IM3](https://user-images.githubusercontent.com/94219582/225509370-15a8af8b-ecd7-40de-9f82-60e9fa38266b.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


