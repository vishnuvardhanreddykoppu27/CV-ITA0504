import cv2
import matplotlib.pyplot as plt

def analyze_color_histogram(image_path):
    # Load the image
    img = cv2.imread(image_path)
    if img is None:
        print(f"Could not open or find the image '{image_path}'. Please check the path.")
        return
# Run the function on 'image car.avif'
analyze_color_histogram('image car.avif')
