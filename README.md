# OpenCV Morphological Operations

This project demonstrates the use of basic **morphological operations** in image processing with **OpenCV**. Morphological operations are commonly used in binary images to process and manipulate the structure of objects.

## Overview

Morphological operations are techniques that process images based on their shape. These operations are particularly useful for tasks like noise removal, object detection, and image enhancement. This project includes implementations of common morphological operations such as **Erosion**, **Dilation**, **Opening**, **Closing**, **Gradient**, **Top Hat**, and **Black Hat**.
I used this photo
<br>![morfo](https://github.com/user-attachments/assets/cd1ffe6f-b471-4399-bf2d-ad90e15ceece)


## Operations Implemented

### 1. **Erosion**
   - **Description**: Erosion reduces the size of the white regions in a binary image. It works by replacing each pixel's value with the minimum value of its surrounding pixels within a kernel.
   - **Use Case**: It is used to remove small white regions (noise) or detach connected objects in binary images.
   
     <br>![download](https://github.com/user-attachments/assets/99484360-a45a-4850-ac38-1f0fc5c6d442)


### 2. **Dilation**
   - **Description**: Dilation increases the size of the white regions in a binary image. Each pixel’s value is replaced with the maximum value of its surrounding pixels within a kernel.
   - **Use Case**: It is used to fill small holes in the foreground or expand objects.
   
     <br>![download](https://github.com/user-attachments/assets/e5797e48-1744-4ef0-a359-4ab6eb64fe27)
     <br>![download](https://github.com/user-attachments/assets/4b01e1dd-7a54-4688-b7dc-88dabc7a3e79)


### 3. **Opening**
   - **Description**: Opening is the process of first performing an erosion followed by dilation. This operation is useful for removing small noise from an image.
   - **Use Case**: It is effective for cleaning up small artifacts in an image.

     <br>![download](https://github.com/user-attachments/assets/bf503aed-e534-472d-8d0f-0e398b1f460b)
     <br>![download](https://github.com/user-attachments/assets/ebbe7dbb-730f-4228-a619-2151aa426ae5)

### 4. **Closing**
   - **Description**: Closing is the process of first performing dilation followed by erosion. This operation is useful for filling small holes or gaps in the image.
   - **Use Case**: It is used to close small dark regions or holes within objects.

     <br>![download](https://github.com/user-attachments/assets/36bdaaee-4ae3-44ee-a006-0477b8662e34)


### 5. **Gradient**
   - **Description**: The gradient is the difference between dilation and erosion. This operation highlights the edges in an image.
   - **Use Case**: It is commonly used for edge detection.

     <br>![download](https://github.com/user-attachments/assets/e4a9c4b2-cf0f-49b3-abf5-cebd4f845e0e)


### 6. **Top Hat**
   - **Description**: Top Hat is the difference between the original image and the result of opening the image. It highlights small objects in the foreground.
   - **Use Case**: It is useful for detecting small objects or enhancements in a binary image.


### 7. **Black Hat**
   - **Description**: Black Hat is the difference between the closing operation and the original image. It highlights the background features.
   - **Use Case**: It is used to extract dark features or background objects in an image.

     <br>![download](https://github.com/user-attachments/assets/370848d3-69cd-4d6a-80f0-97c5089933b3)

<br>

## Requirements

- Python 3.x
- `opencv-python`
- `numpy`
- `matplotlib`

You can install the required libraries using the following command:

```bash
pip install -r requirements.txt
