import cv2
from google.colab.patches import cv2_imshow

# Read the uploaded image
image_path = "image car.avif"
image = cv2.imread(image_path)

if image is None:
    print(f"Could not load the image: {image_path}. Please check if the file name is correct.")
else:
    # Convert the image to grayscale
    gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
