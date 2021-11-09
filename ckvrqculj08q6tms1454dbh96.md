## Python - OpenCV library for image and video analysis

Hey techies! I believe for you to be here, you either write python codes and you are interested in knowing the exciting function that the OpenCV library in python does, or you write other programming languages and you have a perspicacity for this topic. Whichever, I'm super excited to walk you through!

### KEY TAKEAWAYS
-  **Concept of OpenCV**
-  **Applications of OpenCV**
-  **How to install the OpenCV library in python **
-  **How does the OpenCV library work? **
-  **Building an IMAGE BLURRING application with python!**😊

Excited🎉? Let's dive in!

### CONCEPT OF OpenCV
OpenCV is an acronym for Open **C**omputer** V**ision. It is an open-source library in python, that typically analyzes images and videos. OpenCV is a part of the Artificial Intelligence field that is trained to allow computers to work with images and videos just like humans. 

OpenCV was first developed by intel in 1999 with C/C++ programming, later, it was integrated into other languages including python!

### APPLICATIONS OF OpenCV 
OpenCV has a lot of pre-trained classifiers that can be used to identify objects such as shapes, number plates, faces, objects, etc. We can use these classifiers to detect an object based on what we want to use it for. There are several applications of the OpenCV, some of which include:

1. Object Detector
2. Image Processing
3. Face detector
4. Face recognition
5. Handwriting Recognition
6. Advance robotic vision
7. License plate reading and many others...

### HOW TO INSTALL THE OpenCV LIBRARY IN PYTHON
**STEP 1:** 
Be sure you have python and pip pre-installed on your PC. If you don't, download Python [here](https://www.python.org/). 

> The newest versions of Python already have pip in them so you do not have to install pip separately.

 To confirm for Python, type:

```python --version```


To confirm for pip, type:

```pip -V``` 

**STEP 2:** 
Install OpenCV. The following command can be used to install OpenCV using pip;


```pip install opencv-python``` 


This command will start downloading and installing packages related to the OpenCV library. Once it is completed, a success message of installation will be displayed.

![frame_generic_light.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1636438794833/lEu5e2rJ6.png)

**STEP 3 (not required):**
In OpenCV projects, you may find that you'll be using Number systems a lot, I recommend you use the Numpy library. NumPy provides a multidimensional array object, as well as variations such as masks and matrices. You can install NumPy by entering the following into your terminal

```pip install Numpy```

**STEP 4 (not required):** Install Matplotlib. It is an Application Programming Interface that consists of functions that help process data for visualization. You can install Matplotlib by entering the following into your terminal

```pip install Matplotlib```

### HOW DOES THE OpenCV LIBRARY WORK?
OpenCV can define colors, read and write images from scratch, draw an image through code, capture and save videos, process images, perform feature detection, detect specific objects and analyze videos, and determine the direction and the motion of an object.

### BUILDING AN IMAGE BLURRING APPLICATION WITH PYTHON🎉
The most basic things to know to process an image or video are to read, show and write images, while other code, functions, and libraries that may be attached in this process are dependencies and can be complex depending on how large the project you are working on is.

```
import cv2
import numpy as np
from matplotlib import pyplot as pypt

#Make sure the image you are reading is in your working directory
img = cv2.imread('watermelon.jpg')

# function to blur image indicating how blur it should be
blur_img = cv2.blur(img,(15,15))

print(pypt.subplot(121),pypt.imshow(img),pypt.title('Original image'))
pypt.xticks([]), pypt.yticks([])
print(pypt.subplot(122),pypt.imshow(blur_img),pypt.title('Blurred image'))
pypt.xticks([]), pypt.yticks([])
print(pypt.show())

```
           
After running the code above, your output should look like this:


![frame_generic_dark (3).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1636404049436/WZU0xebaC.png)

> You can as well have the image on your PC by clicking on the **SAVE** icon beneath the running application! 


### RESOURCES
OpenCV library is an amazing library that makes computer process images and videos just like humans can do.
To advance your studies on Python OpenCV, you can see the official documentation  [here](https://pdfroom.com/books/opencv-python-tutorials-documentation/qlgyyaxmgMG) or check out other resources like;
1. 
<iframe width="100%" height="400" src="https://www.youtube.com/embed/oXlwWbU8l2o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="0">
</iframe>
2.  [edureka.co/blog/python-opencv-tutorial](https://www.edureka.co/blog/python-opencv-tutorial/) 
3.  [geeksforgeeks.org/opencv-python-tutorial](https://www.geeksforgeeks.org/opencv-python-tutorial/#:~:text=OpenCV%20is%20a%20huge%20open,the%20handwriting%20of%20a%20human.) 

I hope you have learned something new today! I'll like to read your feedback from the comment section below. Also, you can reach out to me on [LinkedIn](https://linkedin.com/in/gracesoyebi), I love to connect with you all.






