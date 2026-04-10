# 📵 Workplace Mobile Usage Detection

An object detection system that identifies unauthorised mobile phone usage in the workplace using Computer Vision and Deep Learning — built to enforce organisational compliance and reduce distraction-related productivity loss.

---

## 🎯 Objective

Manual monitoring of mobile phone usage in professional environments is inconsistent and resource-intensive. This project automates the detection of mobile usage through real-time object detection on workplace video feeds, supporting compliance enforcement without continuous human oversight.

---

## 🚀 Features

- **Real-time Mobile Detection** — Detects mobile phone usage by employees in workplace footage
- **Custom-trained Model** — Fine-tuned on a domain-specific dataset of 497 annotated workplace images
- **High Detection Accuracy** — Validated with strong performance metrics on unseen data
- **Fast Inference** — Built on Roboflow 3.0 Object Detection (Fast) architecture for low-latency results
- **Scalable Pipeline** — Modular design supports integration with CCTV feeds or video files

---

## 📊 Model Performance

| Metric     | Score  |
|------------|--------|
| mAP@50     | 85.9%  |
| Precision  | 83.1%  |
| Recall     | 79.0%  |
| F1 Score   | 81.0%  |

> Evaluated on a held-out validation set. Model fine-tuned using **Roboflow 3.0 Object Detection (Fast)**.
<img width="1917" height="858" alt="Mobile Usage Detection" src="https://github.com/user-attachments/assets/ddec5b35-3543-4f6a-8582-b666020474ca" />

---

## 🛠️ Tech Stack

| Tool / Library     | Purpose                              |
|--------------------|--------------------------------------|
| Roboflow           | Dataset management, annotation, training, deployment |
| Roboflow 3.0 (Fast)| Object detection model architecture |
| Python             | Core development language            |
| Jupyter Notebook   | Model development and experimentation |
| OpenCV             | Video/image processing               |
| Ultralytics        | YOLO            |

---

## 🔄 ML Pipeline

```
Data Collection → Annotation (Roboflow) → Dataset Versioning
       ↓
Model Training (Roboflow 3.0 Fast) → Evaluation (mAP, Precision, Recall, F1)
       ↓
Inference on Workplace Video Feeds
```

---

## 📖 Dataset

- **Total Images:** 497 (custom-collected from workplace environment)
- **Classes:** `mobile_phone`
- **Annotation Tool:** Roboflow
- **Dataset Version:** `mobile_detection_v2`
- **Augmentations:** Applied via Roboflow to improve generalisation

---

## 🏢 Applied Context

Developed and validated within **Summer Solutions Pvt. Ltd.** as part of an internal workplace safety and compliance initiative. The model was trained on environment-specific data to ensure reliable performance under real organisational conditions.

---

## 🔗 Related Project

This project is part of a broader **AI-Powered Workplace Safety & Compliance** initiative:

👉 [Pharmaceutical Lab Safety Monitoring](https://github.com/dinesh-paladugula/AI-Powered-Workplace-Safety-and-Compliance-Monitoring) — PPE Detection + Action Recognition using YOLOv11

---

## 📄 License

This project is intended for internal organisational use. Model weights are subject to **AGPL-3.0** as per Roboflow 3.0 licensing terms.

---

## 👤 Author

**Dinesh**  
AI Engineer - Summer Solutions Pvt. Ltd.  
[LinkedIn](https://linkedin.com/in/dineshbabu-paladugula) • [GitHub](https://github.com/dinesh-paladugula)
