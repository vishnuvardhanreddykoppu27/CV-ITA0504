import cv2
import numpy as np
import matplotlib.pyplot as plt

# Read the uploaded image
img = cv2.imread("image car.avif")

if img is None:
    print("Could not open or find the image 'image car.avif'.")
else:
    # Define a kernel for erosion (5x5 rectangular structuring element)
    kernel = np.ones((5, 5), np.uint8)
