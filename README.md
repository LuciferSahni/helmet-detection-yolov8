# 🛡️ Bike Helmet Detection using YOLOv8

This project uses YOLOv8 nano model to detect whether a person on a bike is wearing a helmet or not. It is aimed at improving road safety through real-time compliance monitoring.

## 🔧 Tech Stack
- Python
- Ultralytics YOLOv8
- Google Colab
- Roboflow (for dataset)
- OpenCV (for testing inference)

## 📦 Dataset
The dataset was sourced and preprocessed using Roboflow. It contains two classes:
- `With Helmet`
- `Without Helmet`

## 🚀 How to Train
```python
from ultralytics import YOLO
model = YOLO('yolov8n.pt')
model.train(data='data.yaml', epochs=10, imgsz=640, batch=8)
```

## 🔍 Example Predictions
![example1](sample_predictions/pred1.jpg)
![example2](sample_predictions/pred2.jpg)

## 🧠 Model Accuracy
Achieved ~85% accuracy on validation set. Works in real-time with webcam or video input.

## 👨‍💻 Author
Armaan Sahni — B.Tech CSE (3rd year)
