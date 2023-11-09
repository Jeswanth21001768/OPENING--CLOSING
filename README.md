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
![image](https://github.com/Jeswanth21001768/OPENING--CLOSING/assets/94155480/9f10c3e0-84da-43b8-8f91-9ffaf52a08a4)

### Display the result of the Opening
![image](https://github.com/Jeswanth21001768/OPENING--CLOSING/assets/94155480/0a318fbb-c05d-4445-b505-730d26015d52)

### Display the result of Closing
![image](https://github.com/Jeswanth21001768/OPENING--CLOSING/assets/94155480/11225581-4217-4bf1-87c8-39f983fa84e8)



## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
