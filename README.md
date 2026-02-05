***

# Anomaly Video Detector 📹



## Overview

The Anomaly Video Detector is a sophisticated surveillance tool that leverages deep learning and computer vision to identify and classify anomalous activities in real-time video streams. By integrating state-of-the-art models like YOLOv8 for object detection and MediaPipe for pose estimation, this system can accurately distinguish between normal and suspicious behaviors. This project is ideal for enhancing security systems in various environments, including public spaces, private properties, and commercial establishments.

***

## Key Features ✨

- **Real-Time Anomaly Detection**: Analyzes video streams in real-time to detect and flag unusual activities as they happen.

- **Multi-Class Classification**: Identifies and categorizes a wide range of anomalies, including:

  - Abuse

  - Arrest

  - Arson

  - Burglary

  - Explosion

  - Robbery

  - Shooting

  - Road Accidents

- **High Accuracy**: Utilizes advanced deep learning models like YOLOv8 and a custom-trained C3D model to ensure precise and reliable detection.

- **Scalable Architecture**: Designed to be easily scalable for various applications, from single-camera setups to extensive surveillance networks.

- **Modular Design**: The codebase is organized into distinct modules for feature extraction, model training, and real-time prediction, making it easy to maintain and extend.

***

## How It Works ⚙️

The system processes video frames through a multi-stage pipeline:

1. **Human Detection**: YOLOv8 is employed to accurately detect and track individuals within the video frame.

2. **Pose Estimation**: MediaPipe extracts human keypoints to analyze body language and posture, which are crucial for identifying intentions and actions.

3. **Feature Extraction**: A combination of spatial and temporal features are extracted from the detected human figures and their movements.

4. **Anomaly Classification**: The extracted features are fed into a custom-trained neural network that classifies the observed behavior into one of the predefined anomaly categories.

***

## Technology Stack 🛠️

- **Python**: The core programming language for the project.

- **PyTorch**: The deep learning framework used for model training and deployment.

- **OpenCV**: For real-time video processing and computer vision tasks.

- **YOLOv8**: For high-performance object detection.

- **MediaPipe**: For accurate human pose estimation.

- **Scikit-learn**: For data preprocessing and model evaluation.

- **Jupyter Notebook**: For model development, training, and testing.

***

## Installation and Setup 🚀

To get the Anomaly Video Detector up and running, follow these steps:

1. **Clone the Repository**:

   Bash

   ```
   git clone https://github.com/envisdrako/anomaly-video-detector.git
   cd anomaly-video-detector

   ```

2. Install Dependencies:

   It is recommended to use a virtual environment to manage dependencies.

   Bash

   ```
   pip install -r requirements.txt

   ```

3. Download Pre-trained Models:

   Ensure you have the pre-trained models (final\_model.pth, final\_scaler.joblib, label\_mapping.joblib) in the Save/ directory.

***

## Usage 🎯

To start detecting anomalies in a video file, you can run the `testingv3.ipynb` notebook. Make sure to update the video path in the notebook to point to your desired video file.

For training the model on a new dataset, you can use the `trainingv2.ipynb` notebook. The pipeline for feature extraction from raw videos is detailed in `pipeline.ipynb`.

***


