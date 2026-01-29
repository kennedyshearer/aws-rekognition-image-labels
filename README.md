# AWS Rekognition Image Labels Generator

## 📌 Project Overview
This project demonstrates how to build an image labeling application using **Amazon Rekognition**. Images stored in an **Amazon S3 bucket** are analyzed using Rekognition’s `DetectLabels` API to automatically identify objects, scenes, and concepts within an image, along with confidence scores.

The application is implemented using **Python (Boto3)** and interacts with AWS services via the **AWS CLI**.

---

## 🏗 Architecture Overview

<!-- INSERT ARCHITECTURE DIAGRAM HERE -->
<p align="center">
  <img src="https://i.gyazo.com/b43422461c2f154daaa8ab7c8080ef17.png" alt="Diagram" width="700">
  <br>
  <sub>Figure 1: Architecture Diagram</sub>
</p>

### Architecture Flow
1. Images are uploaded to an Amazon S3 bucket
2. A Python script retrieves the image object from S3
3. Amazon Rekognition analyzes the image using `DetectLabels`
4. Labels and confidence scores are returned and displayed in the terminal

### AWS Services Used
- **Amazon S3** – Image storage
- **Amazon Rekognition** – Image analysis and label detection
- **AWS CLI** – AWS configuration and access
- **AWS IAM** – Permissions and access control

---

## 📝 Prerequisites
- AWS account (Free Tier)
- Python 3.x
- AWS CLI installed and configured
- IAM user or role with:
  - `AmazonRekognitionReadOnlyAccess`
  - `AmazonS3ReadOnlyAccess`

<!-- INSERT AWS CLI CONFIGURATION SCREENSHOT HERE -->

---

## 🚀 Environment Setup

### Install Required Libraries
```bash
pip install boto3

