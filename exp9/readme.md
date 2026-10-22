import cv2
from google.colab.patches import cv2_imshow

# Read your uploaded image
image_path = "Screenshot 2026-10-22 094638.png"
image = cv2.imread(image_path)

if image is not None:
    # Resize to a bigger size (2x scaling) using Bilinear interpolation
    bigger_image = cv2.resize(image, None, fx=2, fy=2, interpolation=cv2.INTER_LINEAR)

else:
    print(f"Error: '{image_path}' could not be loaded. Please check the file path.")
