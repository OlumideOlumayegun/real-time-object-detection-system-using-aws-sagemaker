# 📦 Real-Time Object Detection Using using AWS SageMaker

## 🚀 Overview

This project demonstrates the development of a scalable, end-to-end object detection system using AWS SageMaker. It covers the full machine learning lifecycle, including data preparation, model training, evaluation, deployment, and inference for real-time object detection.

The solution leverages AWS managed services to build a production-ready computer vision pipeline capable of detecting and localising objects in images.

---

## 🧠 Key Features

* End-to-end ML pipeline on AWS SageMaker
* Image data preprocessing and annotation handling
* Training using SageMaker built-in Object Detection algorithm
* Hyperparameter tuning for performance optimisation
* GPU-accelerated training
* Real-time model deployment via SageMaker endpoints
* Scalable inference pipeline
* Modular and reproducible workflow

---

## 🏗️ Architecture

1. Data stored in Amazon S3
2. Data preprocessing and formatting
3. Model training using SageMaker Object Detection algorithm
4. Model artefact storage in S3
5. Deployment to SageMaker endpoint
6. Real-time inference

---

## 📂 Project Structure

```
.
├── notebooks/
│   └── Sagemaker-Object-Detection.ipynb
├── README.md
```

---

## ⚙️ Technologies Used

* AWS SageMaker
* Amazon S3
* Python (Boto3, NumPy, Pandas)
* Deep Learning (Object Detection algorithms)
* Jupyter Notebook

---

## 📊 Model Training

* Algorithm: SageMaker Built-in Object Detection (MXNet-based)
* Metrics: Mean Average Precision (mAP)
* Training Instance: GPU-backed (e.g., ml.p3 / ml.g4dn)
* Hyperparameter tuning applied to improve performance

---

## 🚀 Deployment

The trained model is deployed to a **real-time SageMaker endpoint**, enabling:

* Low-latency predictions
* Scalable inference
* Integration with downstream applications

---

## 🔍 Inference

* Input: Image
* Output: Bounding boxes, class labels, confidence scores

Example output:

```json
{
  "predictions": [
    {
      "class": "object_name",
      "confidence": 0.95,
      "bbox": [x_min, y_min, x_max, y_max]
    }
  ]
}
```

---

## 📈 Results

* Achieved strong object detection performance
* Successfully deployed a production-ready model
* Enabled real-time object detection with scalable infrastructure

---

## 🧪 How to Run

1. Open the notebook in SageMaker Studio / Notebook Instance
2. Execute cells sequentially:

   * Data preparation
   * Training
   * Deployment
3. Test inference using sample images

---

## 🔐 Prerequisites

* AWS Account
* IAM Role with SageMaker & S3 access
* SageMaker Studio or Notebook Instance

---


## 📜 License

This project is licensed under the MIT License.

---
