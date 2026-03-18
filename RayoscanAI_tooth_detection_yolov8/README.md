# RayoscanAI Tooth Detection using YOLOv8

## Overview
This project focuses on detecting and classifying tooth numbers from dental images using a deep learning-based object detection model (YOLOv8). The model identifies each tooth and assigns the correct label.

---

## Dataset
- ~500 dental images
- YOLO format annotations (.txt files)
- 32 classes (tooth numbers 0–31)
- Each image contains multiple labeled teeth
- Split: 80% training, 20% validation

---

## Why YOLOv8
YOLOv8 was selected due to its speed, efficiency, and strong performance in object detection tasks. It performs detection and classification in a single step, making it suitable for real-time applications.

The YOLOv8n (nano) model was used as it provides a good balance between speed and accuracy and is lightweight for training.

---

## Approach
- Prepared dataset in YOLO format
- Split data into training and validation sets (80:20)
- Trained YOLOv8 model on dental images
- Used GPU (T4) in Google Colab for faster training
- Performed inference using trained model
- Evaluated performance using mAP metrics

---

## Model & Training
- Model: YOLOv8n
- Epochs: 50
- Image size: 640
- Framework: Ultralytics YOLO
- Environment: Google Colab (T4 GPU)

---

## Results
- mAP@50 ≈ 0.52  
- mAP@50-95 ≈ 0.33  

The model successfully detects teeth and assigns correct labels. Sample outputs are available in the `outputs/` folder.

---

## Project Structure
Tooth-Detection-YOLOv8/
│── tooth_detection.ipynb
│── weights/
│ └── best.pt
│── outputs/
│── report.pdf
│── README.md

---

## Files Included
- `tooth_detection.ipynb` → Training and prediction code  
- `weights/best.pt` → Trained model  
- `outputs/` → Sample predictions  
- `report.pdf` → Project report  

---

## Conclusion
The YOLOv8 model effectively detects and classifies tooth numbers from dental images. Performance can be improved further with more data and tuning.

---

## Author
**V. Bindu Sri**  
Email: Vadlabindu15@gmail.com