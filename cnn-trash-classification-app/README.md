# Trash Classification using Convolutional Neural Networks (CNN)

This repository is a fork and extension of the [webapp-trash-classification](https://github.com/vladalexey/webapp-trash-classification) project originally developed by [vladalexey](https://github.com/vladalexey). It demonstrates the use of Convolutional Neural Networks (CNNs) to classify images of waste into six categories, with a Flask-based web application enabling real-time image classification.

---

## Project Description

Manual trash sorting is inefficient, error-prone, and labor-intensive. This project explores how deep learning can support smart recycling and waste segregation systems by automating trash classification.

The underlying model is a CNN trained on image data corresponding to various waste types. The trained model is integrated into a lightweight Flask web interface that allows users to upload images and receive predicted labels. This serves as a prototype for real-world deployment in smart waste bins or civic waste collection applications.

This project also includes enhancements and reorganization for clarity and reuse. The application demonstrates how AI techniques can be paired with web technologies to create deployable end-to-end solutions.

---

## My Contributions

This repository has been adapted and refined for learning and portfolio-building purposes. The following contributions were made:

- Refactored and documented existing code for readability and reuse.
- Expanded project structure documentation including this updated README.
- Identified future development areas such as:
  - Transfer learning with pretrained CNN architectures (e.g., ResNet).
  - Cloud/web-based deployment using Streamlit or Hugging Face Spaces.
  - Enhanced UI/UX and webcam support for real-time classification.

---

## Model Summary

- **Architecture**: Basic CNN with 3–4 convolutional layers, ReLU activations, pooling layers, and fully connected output.
- **Input**: Image data normalized and resized to fit model input requirements.
- **Output**: Softmax probabilities across six predefined trash classes.
- **Performance**: Validation accuracy ~85% (subject to data variability and hardware).

---

## Classes

The model classifies uploaded images into the following categories:

- Paper
- Plastic
- Glass
- Metal
- Organic
- Other

---

## Dataset

The dataset used includes labeled image samples across the above six categories. It is preprocessed through resizing and normalization prior to training.

Users may extend this application by augmenting the dataset or incorporating benchmark datasets like TACO or WasteNet for higher performance.

---

## Project Structure

├── garbage-classification/ # CNN model definition and training logic
├── static/img/ # Static assets (images/icons)
├── templates/ # HTML templates for Flask frontend
├── webapp/flask-web.py # Flask backend application
├── data_process.py # Data preprocessing and preparation
├── demo.mov # (Optional) demo recording
└── README.md # Project documentation


---

## Web Application

The web interface is powered by Flask and offers basic interaction functionality. Users can upload an image, which is then passed to the backend CNN model. The model returns a class prediction rendered in the frontend. This demonstrates a complete machine learning workflow: data → model → application → user.

---

## Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/samhitasari05/cnn-trash-classification-app.git
cd cnn-trash-classification-app

2. Install Python dependencies:
pip install -r requirements.txt

3.Launch the application:
python webapp/flask-web.py

4. Visit http://127.0.0.1:5000 in your browser and upload an image to classify.

Future Enhancements
Integrate transfer learning models such as ResNet or MobileNet.

Enable webcam-based real-time trash detection.

Expand dataset with publicly available annotated data.

Deploy using interactive platforms such as Streamlit or Hugging Face Spaces.

Improve frontend accessibility and multilingual support.

Credits & License
This project builds upon the open-source repository webapp-trash-classification, developed by vladalexey. The original code is licensed under the MIT License and reused here for academic and educational purposes with attribution.

This repository is for educational use only and does not claim original authorship of the base implementation. Contributions are limited to reorganization, documentation, and forward-planning for real-world applications.
