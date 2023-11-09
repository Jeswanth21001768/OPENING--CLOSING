# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Read the image

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

### Step6:
Display all the output images

 
## Program:
```
Developed By: Jeswanth S 
Register NO: 212221230042
```
``` Python
# Import the necessary packages
import cv2
import numpy as np



# Create the Text using cv2.putText
img= np.zeros((350,1400),dtype ='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'JESWANTH S',(15,200),font,5,(255),10,cv2.LINE_AA)
cv2.imshow('created_text',img)
cv2.waitKey(0)
cv2.destroyAllWindows()



# Create the structuring element
struct_ele= np.ones((9,9),np.uint8)



# Use Opening operation
opening = cv2.morphologyEx(img,cv2.MORPH_OPEN,struct_ele)
cv2.imshow('Opening',opening)
cv2.waitKey(0)
cv2.destroyAllWindows()




# Use Closing Operation
closing = cv2.morphologyEx(img,cv2.MORPH_CLOSE,struct_ele)
cv2.imshow('Closing',closing)
cv2.waitKey(0)
cv2.destroyAllWindows()




```
## Output:

### Display the input Image
![CRE](https://github.com/JEEVAABI/OPENING--CLOSING/assets/93427098/fcfce43b-4f5a-4b80-be10-f856cc44c846)


### Display the result of the Opening
![OPEN](https://github.com/JEEVAABI/OPENING--CLOSING/assets/93427098/d2a3d189-a4bd-4dec-a2e3-8036a43608f4)

### Display the result of Closing
![CLOSING](https://github.com/JEEVAABI/OPENING--CLOSING/assets/93427098/8abe1624-d27f-475f-a5bc-9d558c3629c0)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
