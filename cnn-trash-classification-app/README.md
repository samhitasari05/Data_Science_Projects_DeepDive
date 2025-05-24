# ♻️ Trash Classification using CNN (with Flask Deployment)

This project is a fork and extension of the [webapp-trash-classification](https://github.com/vladalexey/webapp-trash-classification) repository originally created by [vladalexey](https://github.com/vladalexey). It applies Convolutional Neural Networks (CNNs) to classify images of trash into six categories and includes a Flask-based web application for real-time predictions.

---

## 🌍 Problem Overview

Manual waste sorting is inefficient and prone to human error. This project addresses the need for automated waste classification by using a CNN trained on trash images to assist in environmental management and recycling efforts.

---

## 🧠 My Contributions

As part of my machine learning and deployment journey, I:

- ✅ Refactored and documented the code for better readability
- ✅ Rewrote and expanded the README to clearly explain project goals, structure, and usage
- ✅ Identified future improvement areas including:
  - Transfer learning integration (e.g., ResNet)
  - Public deployment using Streamlit or Hugging Face Spaces
  - UI/UX enhancements and webcam support

---

## 🚀 Demo Screenshot

![App Screenshot](static/img/demo-screenshot.png)

---

## 🛠️ Tech Stack

| Function         | Technology                 |
|------------------|----------------------------|
| Model Training   | PyTorch (originally TensorFlow supported) |
| Image Handling   | OpenCV, NumPy              |
| Web Interface    | Flask, HTML, CSS           |
| Visualization    | Matplotlib (optional)      |

---

## 🧪 Categories Detected

The model predicts one of six categories:

- Paper
- Plastic
- Glass
- Metal
- Organic
- Other

---

## 📁 Project Structure

├── garbage-classification/ # CNN model and training code
├── static/img/ # Image assets
├── templates/ # HTML frontend templates
├── webapp/flask-web.py # Flask app backend
├── data_process.py # Preprocessing script
├── demo.mov # (Optional) Demo video
└── README.md


---

## 🧪 Model Overview

- Architecture: Custom CNN (3–4 convolutional layers)
- Input: Trash images resized and normalized
- Output: Softmax probability across 6 categories
- Performance: ~85% validation accuracy
- Deployment: Real-time image classification through web UI

---

## 🌟 Future Improvements

- 🔄 Switch to a transfer learning model (ResNet, MobileNet)
- 🌐 Deploy with Streamlit, Gradio, or Hugging Face Spaces
- 📷 Add webcam support for live classification
- 🌎 Support multilingual labeling for broader reach
- 📦 Incorporate TACO or WasteNet datasets for improved accuracy

---

## 📄 Credits & License

This repository builds upon the open-source work of [vladalexey](https://github.com/vladalexey) under the [MIT License](LICENSE). All original authorship is retained where applicable.

> **Disclaimer**: I do not claim original authorship of the base code. This fork is intended for educational and personal portfolio purposes with attribution.

---

Explore more at [github.com/samhitasari05](https://github.com/samhitasari05).


