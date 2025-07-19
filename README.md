# Real-Time Emotion Detection using Deep Learning

This repository showcases two distinct approaches to building a real-time facial emotion detection system. The first method involves constructing a Convolutional Neural Network (CNN) from scratch, while the second leverages the pre-built DeepFace library for a faster implementation.

---

## Approach 1: Custom CNN Model with VGG16 Architecture

This project involves the design and implementation of a real-time emotion detection system using a custom Convolutional Neural Network (CNN).

* **Architecture**: The model is built upon the **VGG16** architecture, a powerful and well-regarded CNN structure for image classification. It utilizes key layers including Convolutional Layers for feature extraction, Max-Pooling Layers for dimensionality reduction, and Fully Connected Layers for final classification.
* **Dataset**: The model was trained and validated on the public **FER2013 (Facial Expression Recognition 2013)** dataset. This dataset contains facial images labeled with seven distinct emotion classes: angry, disgust, fear, happy, sad, surprise, and neutral.
* **Performance**: The final model achieved an overall **accuracy of 66%** on the test dataset.

---

## Approach 2: Library-Based Implementation with DeepFace

This method provides a straightforward and rapid implementation of emotion detection by utilizing established computer vision libraries.

* **Face Detection**: The system uses the **Haar Cascades** algorithm from the `OpenCV` library to detect the location of faces in a real-time video feed from a webcam.
* **Emotion Analysis**: Once a face is detected, the `DeepFace` library is used to analyze the facial region and identify the dominant emotion.

---

## 🚀 How to Run the Project

1.  **Clone the Repository**
    ```bash
    git clone [your-repository-url]
    cd [your-repository-folder]
    ```

2.  **Create and Activate a Virtual Environment**
    ```bash
    # Create the environment
    python -m venv venv
    # Activate on Windows
    venv\Scripts\activate
    # Activate on macOS/Linux
    source venv/bin/activate
    ```

3.  **Install Required Libraries**
    Ensure the `requirements.txt` file is in your project directory.
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Notebooks**
    Open and run the cells within either of the Jupyter Notebook files (`.ipynb`) to see each approach in action.

---

## 🛠️ Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* DeepFace
* Numpy
* Matplotlib