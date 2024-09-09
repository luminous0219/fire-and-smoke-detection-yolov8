![Fire Detection Demo](https://github.com/luminous0219/fire-and-smoke-detection-yolov8/blob/main/fire%20demo%201.gif)
![Fire Detection Demo](https://github.com/luminous0219/fire-and-smoke-detection-yolov8/blob/main/fire%20demo%202.gif)

**Fire and Smoke Detection Model**

This repository contains a trained model for fire and smoke detection using the Ultralytics YOLOv8 architecture. The model has been fine-tuned to detect fire and smoke in video files and images with high accuracy and can be integrated into various applications such as surveillance systems, disaster monitoring, and safety systems.

**Model Information**

Architecture: YOLOv8n (Nano) - optimized for high speed and efficiency
Trained On: Custom dataset of fire and smoke images https://universe.roboflow.com/fire-rqbio/fire-and-smoke-yikzn

Detection Capabilities:
Fire
Smoke

**Features**
Real-time fire and smoke detection
Lightweight and efficient, suitable for deployment on edge devices
Can be used with video streams or image inputs
Configurable confidence and IoU thresholds for fine-tuning detection sensitivity

Usage
1. Loading the Model
You can load the pre-trained model using Ultralytics YOLOv8 library or PyTorch:

from ultralytics import YOLO

# Load the custom-trained fire and smoke model
model = YOLO("best.pt")

2. Running Inference on an Image or Video
To run inference on an image or video, use the following code:

Inference on an image
results = model("path_to_image.jpg")
results.show()

Inference on a video file
results = model("path_to_video.mp4")
results.show()

3. Deployment
The model can be deployed in various environments such as:

Web applications: Integrated with Gradio or Streamlit for creating an interactive web interface.
Mobile apps: Utilize the model with mobile cameras for fire and smoke detection.
Edge devices: Deploy the model on devices with limited resources for real-time detection.
