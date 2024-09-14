<H3>Name: SACHIN C </H3>
<H3>Register no: 212222230125</H3>
<H3>Date: 14.9.24 </H3>

# WORKING ON AN IMAGE

# PROGRAM:
```python
import cv2
import matplotlib.pyplot as plt

image1 = cv2.imread('image1.png')
image2 = cv2.imread('image2.jpg')

image1.shape
image2.shape

image1_resized = cv2.resize(image1, (400,400))
image2_resized = cv2.resize(image2, (400,400))
image1_resized.shape
image2_resized.shape

R1 = image1_resized[0:200, 0:200]
R2 = image1_resized[0:200, 200:400]
R3 = image1_resized[200:400, 0:200]
R4 = image1_resized[200:400, 200:400]
R5 = image2_resized[0:200, 0:200]
R6 = image2_resized[0:200, 200:400]
R7 = image2_resized[200:400, 0:200]
R8 = image2_resized[200:400, 200:400]
image1_resized[0:200, 0:200] = R8
image2_resized[200:400, 200:400] = R3
plt.imshow(image1_resized)
plt.show()
plt.imshow(image2_resized)
plt.show()
```

# OUTPUT:

![image](https://github.com/user-attachments/assets/677f2ae8-1e61-4577-9460-f35716fcaf3b)

![image](https://github.com/user-attachments/assets/52a48eb6-8ec2-4bbc-967f-813cb51b536c)

 
