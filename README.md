# 🚦 Traffic Vehicle Detection and Analysis Using YOLOv8

## 📌 Project Overview

This project implements an end-to-end **vehicle detection and traffic analysis pipeline** using computer vision. A pre-trained **YOLOv8 object detection model** is applied to long-duration traffic videos (14 minutes) to detect and classify vehicles into:

- Car  
- Bus  
- Truck  
- Motorcycle  

The system processes raw traffic videos, generates **annotated videos with bounding boxes**, and converts detections into a structured **CSV dataset** for analysis.

---

## 🎯 Problem Statement

Traffic monitoring plays a critical role in:

- Urban planning  
- Congestion reduction  
- Road safety improvement  
- Smart city development  

Traditional traffic counting methods (manual observation or physical sensors) are costly and limited in scalability. This project demonstrates how **computer vision-based object detection** can automate vehicle counting and traffic flow analysis using video data.

---

## 🧠 Objectives

- Detect vehicles in traffic videos using YOLOv8  
- Generate annotated output videos  
- Extract per-frame vehicle counts  
- Convert detections into structured CSV format  
- Perform exploratory data analysis (EDA) on traffic distribution  

---

## 📂 Dataset

- Traffic surveillance videos (~14 minutes long)
- Fixed camera viewpoint
- Real-world urban road conditions
- One primary video used for detailed analysis to reduce misclassification noise

---

## 🛠️ Methodology

### 1️⃣ Object Detection
- Used pre-trained YOLOv8 model
- Processed full-length traffic video
- Generated annotated video with bounding boxes and class labels

### 2️⃣ Data Extraction
For each frame, the following were recorded:
- Frame number
- Car count
- Bus count
- Truck count
- Motorcycle count

### 3️⃣ Data Transformation
The dataset was reshaped into a structured format suitable for analysis:


This format enables flexible aggregation and visualization.

---

## 📊 Exploratory Data Analysis (EDA)

<img width="713" height="451" alt="image" src="https://github.com/user-attachments/assets/20ee09df-5a31-4904-9dac-92d9721e171a" />


Key findings:

- Cars dominate traffic flow (realistic urban distribution)
- Trucks and buses appear less frequently
- Minor misclassification observed (e.g., truck labeled as bus)
- Traffic density varies across timeframes

Vehicle distribution summary:

- Car: 23,903  
- Truck: 1,537  
- Bus: 203  
- Motorcycle: 0  

The model performed well overall given that it was not fine-tuned on a custom dataset.

---

## 🎥 Annotated Video Results

Due to GitHub's 100MB file size limit, full annotated videos are hosted externally:

🔗 **Full Annotated Videos:**  

https://drive.google.com/file/d/1kYQatNM5yo6BkG0d2a-IEjsgGz0e09sV/view?usp=drive_link

https://drive.google.com/file/d/1Kx5UJXWmtT2SzR2I4JZiNS-uFEgDBzLS/view?usp=drive_link

https://drive.google.com/file/d/1re7jONwe9k73x_srDzTu3lBVBC3hWSDX/view?usp=drive_link



📌 A short demo clip is included in this repository for preview purposes.



---

## ⚠️ Limitations

- Minor confusion between visually similar classes (bus vs truck)
- No custom fine-tuning performed
- Detection accuracy depends on camera angle and lighting

---

## 🔮 Future Improvements

- Fine-tune YOLOv8 on a custom traffic dataset  
- Improve class balancing  
- Add real-time streaming support  
- Integrate interactive traffic analytics dashboard  
- Implement vehicle tracking (not just detection)  

---

## 🧑‍💻 Technologies Used

- Python  
- YOLOv8 (Ultralytics)  
- OpenCV  
- Pandas  
- Matplotlib / Seaborn  


---

## 📌 Conclusion

This project demonstrates a complete **computer vision pipeline for automated traffic monitoring**, from raw video input to structured data insights. It highlights the practical application of object detection models in real-world urban traffic analysis.

---

## 👤 Author

Kenneth Nyangweso
Computer Vision | Data Analytics | Machine Learning
