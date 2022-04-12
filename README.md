# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import cv2 and save and image as filename.jpg

### Step2:
Use imread(filename, flags) to read the file.

### Step3:
Use cv2.cvtColor(src, code, dst, dstCn) to convert an image from one color space to another

### Step4:
Split and merge the image using cv2.split and cv2.merge commands

### Step5:
End the program and close the output image windows.

## Program:
```python
# Developed By: Lishali Ramamoorthy 
# Register Number: 212220230028
# i) Convert BGR and RGB to HSV and GRAY
import cv2
color_image = cv2.imread('images.png')
plt.imshow(color_image)
plt.show()
hsv_image = cv2.cvtColor(color_image, cv2.COLOR_BGR2HSV)
plt.imshow(hsv_image )
plt.show()
gray_image1 = cv2.cvtColor (color_image, cv2.COLOR_RGB2GRAY)
plt.imshow(gray_image1)
plt.show()




# ii)Convert HSV to RGB and BGR

import cv2
color_image = cv2.imread('1.jpeg')
plt.imshow(color_image)
plt.show()
hsv_image = cv2.cvtColor(color_image, cv2.COLOR_HSV2RGB)
plt.imshow(hsv_image )
plt.show()
gray_image1 = cv2.cvtColor (color_image, cv2.COLOR_HSV2BGR)
plt.imshow(gray_image1)
plt.show()



# iii)Convert RGB and BGR to YCrCb

import cv2
color_image = cv2.imread('1.jpeg')
plt.imshow(color_image)
plt.show()
gray_image1 = cv2.cvtColor (color_image, cv2.COLOR_RGB2YCrCb)
plt.imshow(gray_image1)
plt.show()
gray_image1 = cv2.cvtColor (color_image, cv2.COLOR_BGR2YCrCb)
plt.imshow( gray_image1)
plt.show()


# iv)Split and Merge RGB Image

import cv2
color_image = cv2.imread('1.jpeg')
plt.imshow(color_image)
plt.show()
gray_image1 = cv2.cvtColor (color_image, cv2.COLOR_RGB2YCrCb)
plt.imshow(gray_image1)
plt.show()
gray_image1 = cv2.cvtColor (color_image, cv2.COLOR_BGR2YCrCb)
plt.imshow( gray_image1)
plt.show()


# v) Split and merge HSV Image

import cv2
image = cv2.imread('1.jpeg')
hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
plt.imshow(h)
plt.show()
plt.imshow(s)
plt.show()
plt.imshow(v)
plt.show()
Merged_HSV = cv2.merge((h,s,v))
plt.imshow(Merged_HSV)
plt.show()




```
## Output:
### i) BGR and RGB to HSV and GRAY
![image](https://user-images.githubusercontent.com/75235128/162994001-637137f1-db74-4eca-a8f9-fed66bc20110.png)


### ii) HSV to RGB and BGR
![image](https://user-images.githubusercontent.com/75235128/162994036-876ebfcb-fefc-41e6-a0a4-3509111c5c0a.png)

### iii) RGB and BGR to YCrCb
![image](https://user-images.githubusercontent.com/75235128/162994067-8f6ae277-9aa3-452d-a7b2-51117e5e6993.png)

### iv) Split and merge RGB Image
![image](https://user-images.githubusercontent.com/75235128/162994180-9c0cce1b-3172-413d-a2d4-2e3914d33a9e.png)


### v) Split and merge HSV Image
![image](https://user-images.githubusercontent.com/75235128/162994241-1d20ce79-c5b1-4413-9829-6c913d845c62.png)

## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
