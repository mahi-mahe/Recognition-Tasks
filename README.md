# Recognition-Tasks
Aim is to explore and perform different tasks like template matching, shape matching, face detection, mini projects, etc.
Computer Vision Labs – Template Matching, Shape Matching & Face Detection
This repository contains multiple hands‑on projects demonstrating classical computer vision techniques using OpenCV and MediaPipe. The labs are designed for students and practitioners to explore template matching, shape classification, and face detection pipelines.

📌 Lab 1: Template Matching
Objective
Detect a logo/sticker in product photos using normalized cross‑correlation.

Features
Template matching with cv2.matchTemplate

Locate best match using cv2.minMaxLoc

Draw bounding boxes around detected logos

Example
python
result = cv2.matchTemplate(imageGray, templateGray, cv2.TM_CCOEFF_NORMED)
(minVal, maxVal, minLoc, maxLoc) = cv2.minMaxLoc(result)
📌 Lab 2: Shape Matching
Objective
Classify simple shapes (circle, square, triangle) using Hu moments and contour matching.

Features
Extract contours with cv2.findContours

Compute Hu moments for shape descriptors

Match input shapes against template contours with cv2.matchShapes

Annotate detected shapes with labels

📌 Lab 3: Face Detection (Haar Cascade & Webcam)
Objective
Detect faces in group photos and webcam streams using Haar cascades.

Features
Load Haar cascade classifier (haarcascade_frontalface_default.xml)

Detect faces with detectMultiScale

Draw bounding boxes around detected faces

Count faces in group photos

Real‑time webcam capture in Colab

📌 Lab 4: LEGO Brick Detector
Objective
Detect LEGO bricks in a scene using template matching + contour filtering.

Features
Adaptive thresholding for robust segmentation

Contour extraction and filtering by area

Rotation‑invariant template matching (0°, 90°, 180°, 270°)

Non‑maxima suppression (NMS) to remove overlapping detections

Annotated output with bounding boxes and match scores

📌 Lab 5: Haar Cascade vs. MediaPipe Face Detection
Objective
Compare Haar cascades with MediaPipe deep learning detector on the same video.

Results
Speed: Haar Cascade ~0.47 FPS vs. MediaPipe ~13.58 FPS (≈28× faster).

Accuracy: Haar Cascade produced more false positives; MediaPipe was more precise and consistent.

Conclusion: MediaPipe significantly outperforms Haar Cascade in both speed and practical accuracy, making it more suitable for real‑time systems.

🚀 How to Run
Clone the repository:

bash
git clone https://github.com/yourusername/computer-vision-labs.git
cd computer-vision-labs
Install dependencies:

bash
pip install opencv-python matplotlib mediapipe numpy
Run each lab in Google Colab or locally with Python 3.

Upload sample images/videos as required.

🙌 Credits
Built with OpenCV and MediaPipe.

Inspired by classical computer vision labs and modern deep learning detectors.
