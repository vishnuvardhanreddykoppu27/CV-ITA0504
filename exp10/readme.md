import cv2
from google.colab.patches import cv2_imshow

# Load your uploaded image
image_path = "Screenshot 2026-10-22 094638.png"
img = cv2.imread(image_path)

if img is not None:
    # Rotate 90 degrees clockwise
    rotated_img = cv2.rotate(img, cv2.ROTATE_90_CLOCKWISE)

else:
    print(f"Error: '{image_path}' could not be loaded. Please check the file path.")
