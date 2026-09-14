# Opening and Closing Operations Using OpenCV

## Aim

To write a Python program using OpenCV to perform morphological Opening and Closing operations on an image.

The program performs the following operations:

- Morphological Opening
- Morphological Closing

## Software Used

- Anaconda – Python 3.7
- Jupyter Notebook / VS Code
- OpenCV (cv2)
- NumPy
- Matplotlib

## Algorithm

### Step 1:

Import the required libraries: OpenCV, NumPy, and Matplotlib.

### Step 2:

Create or load an input image containing foreground objects.

### Step 3:

Display the original image.

### Step 4:

Create a structuring element (kernel) of suitable size.

### Step 5: Opening Operation

- Apply the Opening operation using the structuring element.
- Opening consists of Erosion followed by Dilation.
- Remove small foreground noises while preserving the shape of larger objects.
- Display the opened image.

### Step 6: Closing Operation

- Apply the Closing operation using the structuring element.
- Closing consists of Dilation followed by Erosion.
- Fill small holes and gaps within foreground objects.
- Display the closed image.

### Step 7:

Compare the original, opened, and closed images.

## Program

## Developed By

**Name:** HARISH S

**Register No:** 212224240052

## Output
## PROGRAM
```
import cv2
import numpy as np
from matplotlib import pyplot as plt
def load_img():
    blank_img =np.zeros((200,200))
    font = cv2.FONT_HERSHEY_SIMPLEX
    cv2.putText(blank_img,text='MI',org=(10,175), fontFace=font,fontScale= 5,color=(255,255,255),thickness=25,lineType=cv2.LINE_AA)
    return blank_img
def display_img(img):
    fig = plt.figure(figsize=(12,10))
    ax = fig.add_subplot(111)
    ax.imshow(img,cmap='gray')
    plt.show()
```

### Original Image

<img width="826" height="817" alt="download" src="https://github.com/user-attachments/assets/3b1fb6e7-f703-468f-9002-036d796887fa" />


### Opening Operation
<img width="826" height="817" alt="download" src="https://github.com/user-attachments/assets/1bf80e2e-26cc-4d92-8c22-71ec72ac1bf5" />

### Closing Operation

<img width="826" height="817" alt="download" src="https://github.com/user-attachments/assets/4d325440-f187-439d-8a22-164bbebbc53d" />
## Applications

### Opening

- Noise removal in binary images.
- Separation of connected objects.
- Preprocessing for object detection.

### Closing

- Filling small holes in objects.
- Connecting nearby components.
- Enhancing segmented regions.

## Advantages

### Opening

- Removes unwanted foreground noise.
- Preserves major object structures.
- Improves segmentation quality.

### Closing

- Restores object continuity.
- Eliminates small background gaps.
- Improves object representation.

## Result

Thus, the morphological operations **Opening** and **Closing** are successfully implemented using OpenCV. 
