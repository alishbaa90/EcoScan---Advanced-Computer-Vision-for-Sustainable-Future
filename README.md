# ♻️ EcoScan - Advanced Computer Vision for Sustainable Future
EcoScan is a browser-native vision intelligence tool designed to automate waste segregation. By implementing a custom YOLO (You Only Look Once) architecture optimized for the web, the application provides high-speed, localized material identification across 44 distinct categories.

## 🚀 Features
- On-Device Inference: Performs all neural processing locally in the browser via TensorFlow.js, ensuring zero data latency and maximum user privacy.
- Custom YOLOv8 Model: Utilizes a lightweight version of the YOLO architecture, specifically trained to recognize complex waste textures and shapes.
- Granular Classification: Successfully identifies 44 specific material types, including various plastics (HDPE, PET), metals (Aluminum, Tin), and organics.
- High-Performance UI: Features a modern, glassmorphic dashboard built with Plus Jakarta Sans, designed for industrial and consumer use cases.

## 🛠️ Technical Stack
- Architecture: YOLO (Object Detection)
- Engine: TensorFlow.js
- Frontend: HTML5, Modern CSS (Grid/Flexbox, Backdrop-filters)
- Inference Type: Edge-AI (Client-side)

## ⚙️ How It Works
- Lexical Processing: The engine initializes the TensorFlow graph model upon page load.
- Pixel Transformation: Uploaded images are resized to a $640 \times 640$ tensor and normalized for the neural network.
- YOLO Inference: The model performs a single pass over the image to extract features and predict class probabilities.
- Result Mapping: The output tensor is parsed, mapped against the 44-label array, and displayed with a confidence score.

## 🖼️ Screenshots
<img width="1366" height="639" alt="Image" src="https://github.com/user-attachments/assets/3923f974-175b-4167-9369-0618274bf3c6" />

<img width="1366" height="628" alt="Image" src="https://github.com/user-attachments/assets/449ff1b9-0fc7-4420-b6c9-2f195aa05444" />

<img width="1366" height="630" alt="Image" src="https://github.com/user-attachments/assets/bbf0ebcd-cc76-488e-b946-9f29be3067d2" />
