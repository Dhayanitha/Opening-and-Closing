# OPENING AND CLOSING

## AIM:
To implement Opening and Closing using Python and OpenCV.

## SOFTWARE REQUIRED:
1. Anaconda - Python 3.7
2. OpenCV
## ALGORITHM:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Use Opening operation.
### Step 5:
Use Closing Operation.

<br><br><br><br><br>

# PROGRAM:
## Developed by   : H.Dhayanitha
## Register Number: 212220230010

# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'DHAYA',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()
```
# Create the structuring element
```
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))
```
# Use Opening operation
```
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()
```
# Use Closing Operation
```
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()

```
## OUTPUT:

### Display the input Image

![d1](https://user-images.githubusercontent.com/75235032/170884384-c331567c-dc97-462f-87b4-2d56e05fdc1b.jpg)

### Display the result of Opening

![d2](https://user-images.githubusercontent.com/75235032/170884388-1190fcb4-8c9b-450d-ac5e-67f9cbf15c73.jpg)

### Display the result of Closing

![d3](https://user-images.githubusercontent.com/75235032/170884404-ea2da8db-85d1-42b6-9eba-15b23997e25d.jpg)

## RESULT:
Thus the Opening and Closing operation is used in the image using python and OpenCV.
