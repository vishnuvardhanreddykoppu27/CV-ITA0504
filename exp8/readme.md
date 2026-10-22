import cv2
from google.colab.patches import cv2_imshow

# Load your uploaded image
image_path = "Screenshot 2026-10-22 094638.png"
image = cv2.imread(image_path) 

if image is not None:
    # Convert the image to grayscale
    gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
else:
    print(f"Error: '{image_path}' could not be loaded. Please check the file path.")
