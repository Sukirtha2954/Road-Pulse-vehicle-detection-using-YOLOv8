# **Road-Pulse Vehicle Detection using YOLOv8**

## **Overview**

The "Road-Pulse Vehicle Detection" project leverages state-of-the-art deep learning models to accurately detect vehicles and monitor traffic congestion levels in urban environments. By combining the power of YOLOv5 and YOLOv8 with an MLP Regressor, this project aims to provide real-time insights into traffic patterns using the KITTI Vision Benchmark Suite and Cityscapes datasets.

## **Project Components**

### **1. Convolutional Neural Networks (CNNs)**
- **YOLOv5 and YOLOv8**: These models are utilized for vehicle detection. YOLO (You Only Look Once) is a fast and accurate object detection algorithm that processes images in real-time to identify vehicles within a given frame.

### **2. Regressor**
- **MLP Regressor**: A Multi-Layer Perceptron (MLP) Regressor is employed to estimate traffic congestion levels based on the detected vehicles. The regressor takes features extracted from the CNN as input to predict congestion severity.

### **3. Datasets**
- **KITTI Vision Benchmark Suite**: This dataset provides high-quality images for object detection, with a focus on vehicles in an urban setting.
- **Cityscapes Dataset**: This dataset is used to augment the model's ability to handle various urban environments, with diverse scenarios and weather conditions.

## **How It Works**

### **Vehicle Detection**:
The YOLOv5 and YOLOv8 models are trained on the KITTI and Cityscapes datasets to detect vehicles in real-time from video streams or images. The models can identify multiple vehicles in a single frame with high precision.

### **Traffic Congestion Monitoring**:
Once vehicles are detected, features such as vehicle count, position, and movement are extracted. These features are fed into the MLP Regressor, which analyzes them to estimate the level of traffic congestion. The model outputs a congestion level score that can be used to monitor and manage traffic conditions in real-time.
