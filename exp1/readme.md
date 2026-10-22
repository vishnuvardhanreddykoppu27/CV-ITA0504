import cv2
from google.colab.patches import cv2_imshow

# Read the uploaded avif image
img = cv2.imread("image car.avif")

# Check whether the image is loaded
if img is None:
    print("Image not found!")
else:
    # Convert image to grayscale
    gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

