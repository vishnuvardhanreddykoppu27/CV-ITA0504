import cv2
from google.colab.patches import cv2_imshow

# Read the uploaded image
img = cv2.imread("image car.avif")

if img is None:
    print("Could not open or find the image.")
else:
    # Apply Gaussian Blur
    # (15, 15) is the kernel size (must be odd numbers). Larger values yield more blur.
    # 0 represents the standard deviation in X direction (auto-calculated when set to 0)
    blurred_img = cv2.GaussianBlur(img, (15, 15), 0)

    # Display the results
    print("Original Image:")
    cv2_imshow(img)

    print("Blurred Image (Gaussian Blur 15x15):")
    cv2_imshow(blurred_img)
