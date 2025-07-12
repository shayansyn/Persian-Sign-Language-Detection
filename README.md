# Real-Time Persian Sign Language Detection (v1.0 - Proof of Concept)

This project is a proof-of-concept for a real-time object detection model, built with the TensorFlow 2 Object Detection API, to recognize and translate Persian Sign Language (PSL) gestures via webcam.

**[Project Status: Active Development & Open to Collaboration]**

![Project Demo GIF](https://i.imgur.com/placeholder.gif)  
*(Demo GIF to be added shortly. This will showcase the model detecting signs in real-time.)*

---

## 🌟 Overview

The goal of this project is to create a system capable of understanding a subset of Persian Sign Language and displaying the corresponding text. This serves as a foundation for building more complex assistive technologies for the deaf and hard-of-hearing community.

While the current model is trained on a custom dataset for four specific Persian words ("من", "باید", "رفتن", "خونه"), the underlying framework is highly adaptable. It can be easily retrained and scaled to support a wider vocabulary, other sign languages, or even entirely different object detection tasks.

---

## ✨ Features

- **Real-Time Detection:** Recognizes sign language gestures instantly via webcam.
- **Custom Dataset:** A unique dataset was built from scratch for Persian Sign Language.
- **Transfer Learning:** Fine-tuned on a pre-trained SSD MobileNetV2 FPNLite model for efficient performance.
- **Scalable Framework:** The architecture allows for easy expansion with more signs and languages.

---

## 🛠️ Technologies Used

- **Python 3.8**
- **TensorFlow 2.10**
- **OpenCV** for image capture and processing.
- **TensorFlow Object Detection API** for the core detection framework.
- **Roboflow** for dataset annotation, augmentation, and management.
- **Jupyter Notebook** for the development and training workflow.

---

## 🖼️ Dataset Samples

Here are sample images from our custom dataset for the four implemented signs.

| من (I/Me) | باید (Must/Should) | رفتن (To Go) | خونه (Home) |
| :---: | :---: | :---: | :---: |
| *(Image Placeholder)* | *(Image Placeholder)* | *(Image Placeholder)* | *(Image Placeholder)* |

*(High-quality sample images will be added here soon.)*

---

## 🚀 How to Run This Project

### Prerequisites

- **Conda (Anaconda or Miniconda) is highly recommended** to manage the complex dependencies of this project.
- A webcam.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/shayansyn/Persian-Sign-Language-Detection.git
    cd Persian-Sign-Language-Detection
    ```

2.  **Create and activate the Conda environment:**
    This project includes a specification file to replicate the exact environment it was developed in.
    ```bash
    # Create the environment from the explicit specification file
    conda create --name psl-detection --file venv_explicit.txt 
    
    # Activate the environment
    conda activate psl-detection
    ```
    *(Note: The `venv_explicit.txt` file is included in this repository.)*

3.  **Download Pre-trained Model Checkpoint:**
    The fine-tuned model checkpoint is not included in this repository due to its size. A download link will be provided here shortly after the model is hosted.
    
    **[Download Link: To be added]**

### Running the Detection

To run the real-time detection, execute the `Tutorial.ipynb` notebook and run the cells, particularly those in the "Detect in Real-Time" section.

---

## 🔮 Future Work & Vision

This project is the first step towards a larger vision. The roadmap includes:

- [x] **Real-Time Gesture Recognition** (Completed)
- [ ] **Expand Vocabulary:** Add more signs to the dataset for a richer vocabulary.
- [ ] **Sequence to Sentence:** Implement an NLP layer (e.g., using an RNN or Transformer) to form complete sentences from detected signs.
- [ ] **Text-to-Speech (TTS):** Add a feature to convert the translated sentences into audible speech.
- [ ] **Real-Time Text Overlay:** Display the detected word or sentence directly on the live camera feed.
- [ ] **UI/UX Improvement:** Develop a user-friendly graphical interface for the application.

---

## 🙏 Acknowledgments

This project's workflow is heavily based on the excellent tutorial for real-time object detection by **Nicholas Renotte**. His [**GitHub repository**](https://github.com/nicknochnack/RealTimeObjectDetection) provided a streamlined and accessible approach to using the TensorFlow Object Detection API.

---
