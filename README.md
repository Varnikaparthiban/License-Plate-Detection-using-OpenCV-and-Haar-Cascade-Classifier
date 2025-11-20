# License-Plate-Detection-using-OpenCV-and-Haar-Cascade-Classifier


### Overview
This repository demonstrates a simple license plate detection pipeline using OpenCV and a Haar Cascade classifier (haarcascade_russian_plate_number.xml). The project contains a Jupyter Notebook that shows how to load an image, run the cascade detector, and visualize results.

This is useful as a learning example or a starting point for building a more complete Automatic Number Plate Recognition (ANPR) system.

### Features
Detects license plate-like regions in images using a pre-trained Haar cascade.
Jupyter Notebook (Lincence_plate_detection.ipynb) with step-by-step code and visualization.
Example image (car.jpg) and cascade file included for quick testing.
Requirements
Python 3.8+ recommended
OpenCV (cv2)
Matplotlib
How it works (brief)
Haar cascades are object detectors trained with positive (object) and negative (non-object) samples. The detectMultiScale() function scans the input image at multiple scales and reports bounding boxes for candidate detections.

### Key parameters to tune:

scaleFactor: Controls image pyramid scaling between passes (e.g., 1.05–1.3).
minNeighbors: Minimum neighbor rectangles needed to keep a detection (higher → fewer false positives).
minSize / maxSize: Limits on detected object size.
Because Haar cascades are simple and fast but less robust than modern deep-learning detectors, results can vary depending on plate style, lighting, angle, and image quality.
