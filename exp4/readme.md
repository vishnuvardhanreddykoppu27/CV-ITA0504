import cv2
import matplotlib.pyplot as plt

# Read the uploaded image
img = cv2.imread("image car.avif")

if img is None:
    print("Could not open or find the image 'image car.avif'. Please ensure the file is in your workspace.")
else:
    # --- 1. Grayscale Histogram Equalization ---
    # Convert the original BGR image to grayscale
    gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
    # Apply histogram equalization to the grayscale image
    gray_equalized = cv2.equalizeHist(gray)
