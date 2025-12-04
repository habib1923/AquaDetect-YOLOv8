# AquaDetect-YOLOv8: Deep Learning-Based Fish Identification

This project implements an object detection model using **YOLOv8 (Ultralytics)** to identify and track various marine life. The model was trained using a custom dataset acquired via Roboflow, focusing on achieving accurate real-time detection for potential industrial or scientific monitoring applications.

## 🎯 Project Goal

To deploy a high-performance computer vision model capable of accurately classifying and locating different species of fish in ocean environments.

## ✨ Key Features

* **Model:** YOLOv8s (pretrained weights)
* **Dataset:** **Ocean-Dataset** from Roboflow, downloaded in YOLOv8 format.
* **Training:** The model was trained for **25 epochs**.
* **Performance (Validation):** Achieved a mean Average Precision (**mAP50-95**) of **0.436**.
* **Hardware Integration:** Designed for use with high-speed imaging hardware, specifically the **Basler daA1440-220um camera** (a high-performance monochrome vision solution).
* **Image Acquisition:** The image acquisition pipeline is set up to use the **pylon SDK**, as indicated by the dependency on `pypylon`.

## 🐟 Detected Classes

The model is trained to detect **8** distinct classes:

1.  Australian Mado
2.  Beau Gregory Damselfish
3.  Bluestriped Goatfish
4.  Burrito Grunt
5.  Monkfish
6.  Narrowband Sergeant Major
7.  Sergeant Major
8.  Silver Batfish

## 🛠️ Setup and Installation

### Dependencies

Ensure you have Python installed, then install the necessary packages.

```bash
pip install ultralytics==8.2.103 roboflow opencv-python matplotlib numpy pyyaml
pip install pypylon  # Required for Basler camera integration
