# Gender-and-Age-Detection-Machine-Learning-.

# Real-Time Age and Gender Detection using OpenCV

This repository contains a real-time computer vision project that predicts a person's age and gender using a live webcam feed. It utilizes OpenCV's Deep Neural Network (DNN) module and pre-trained Caffe models to perform facial recognition and classification. This project serves as a practical demonstration of integrating deep learning models into a real-time application for a data science portfolio.

## Author
**Aryan Tiwari**

## Features
* **Real-Time Face Detection:** Uses an OpenCV face detector to accurately draw bounding boxes around detected faces in a live video stream.
* **Gender Classification:** Predicts gender (`Male` or `Female`) using a pre-trained Caffe model.
* **Age Estimation:** Classifies age into one of eight distinct ranges: `(0-2), (4-6), (8-12), (15-20), (25-32), (38-43), (48-53), (60-100)`.
* **Live Overlay:** Displays the predicted age and gender directly above the bounding box in the active webcam window.

## Prerequisites
To run this project, you need Python installed on your system along with the `opencv-python` library. 

Install the required library using:
`pip install opencv-python`

## Required Model Files
The Jupyter Notebook (`detection.ipynb`) requires the following pre-trained deep learning files in the same directory to function correctly. Ensure these were extracted alongside your notebook:

**Face Detection:**
* `opencv_face_detector.pbtxt`
* `opencv_face_detector_uint8.pb`

**Age Prediction:**
* `age_deploy.prototxt`
* `age_net.caffemodel`

**Gender Prediction:**
* `gender_deploy.prototxt`
* `gender_net.caffemodel`

## How to Run
1.  Clone this repository or extract the project folder to your local machine.
2.  Ensure all the `.pb`, `.pbtxt`, and `.caffemodel` files listed above are stored in the exact same directory as the Jupyter Notebook.
3.  Launch Jupyter Notebook or JupyterLab and open `detection.ipynb`.
4.  Run all the cells sequentially.
5.  Your webcam will activate, and a new window titled "Detecting age and Gender" will pop up.
6.  Look into the camera to see the real-time model predictions.
7.  To exit the application safely and release the webcam, ensure the video window is focused and press the **`q`** key on your keyboard.

## Acknowledgements
This project relies on pre-trained Convolutional Neural Networks (CNNs) for face, age, and gender detection provided by the OpenCV community and respective researchers.
