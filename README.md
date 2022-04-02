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

# Developed By: S. Sanjna Priya
# Register Number: 212220230043
# To Read,display the image
```
import cv2
color_image=cv2.imread('simp.jpg',1)
cv2.imshow('colorimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# To write the image
```
cv2.imwrite('Flower.jpg',color_image)
cv2.imshow('Flower Image',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# Find the shape of the Image
```
import cv2
color_image=cv2.imread('simp.jpg',-1)
print(color_image.shape)
```
# To access rows and columns
```
import cv2
import random
color_img=cv2.imread('simp.jpg',1)
for i in range(150):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
        cv2.imshow('212220230043, S. Sanjna Priya',color_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# To cut and paste portion of image
```
cut=color_image[260:280,100:300]
color_image[60:80,100:300]=cut
cv2.imshow('cutimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## Output:

### i) Read and display the image


![DIP OUT expt1 1](https://user-images.githubusercontent.com/75234965/161382142-1f7cf2ee-a989-437b-8db6-a5ae8d84bbf0.PNG)

### ii)Write the image
![DIP OUT expt1 2](https://user-images.githubusercontent.com/75234965/161382326-39ca352c-40bd-46ff-af64-16e52a5dc16b.PNG)


### iii)Shape of the Image

![DIP OUT expt1 3](https://user-images.githubusercontent.com/75234965/161382041-93d0c556-3e64-46fa-b4af-8eb7d7c85121.PNG)

### iv)Access rows and columns
![DIP OUT expt1 4](https://user-images.githubusercontent.com/75234965/161382056-6dfbedb0-c01e-4bd2-a4af-20656bf1dabd.PNG)

### v)Cut and paste portion of image

![DIP OUT expt1 5](https://user-images.githubusercontent.com/75234965/161382068-c63a5b62-9997-4e83-b57f-6d6b29943f8c.PNG)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


