# Image Classifier with Deep Learning

A deep learning solution for fine-grained flower classification, developed as the capstone project of the **AI Programming with Python and TensorFlow Nanodegree**. The system leverages transfer learning to train a high-accuracy convolutional neural network on the Oxford Flowers dataset, and exposes the trained model through a production-ready command-line interface for real-time inference.

## Project Overview

This repository delivers an end-to-end image classification pipeline, from model development and training to deployment as a standalone prediction tool. The work is organized into two complementary components:

### Part 1 — Model Development (Jupyter Notebook)
- **File:** `Project_Image_Classifier_Project.ipynb`
- Engineered a deep neural network using transfer learning from a pre-trained backbone.
- Configured GPU acceleration to optimize training throughput.
- Implemented a robust data pipeline for loading, preprocessing, and augmenting the flower dataset.
- Fine-tuned model hyperparameters and rigorously evaluated performance against validation and test sets.

### Part 2 — Command-Line Inference Application
- **`predict.py`** — Entry point that loads the trained model and returns predictions for any input image.
- **`utility.py`** — Modular helpers for image preprocessing, label mapping, and model loading.
- **`projUdacity.h5`** — Serialized Keras model exported from Part 1.

The CLI accepts an image path and returns the top-K predicted classes along with their associated probabilities, providing both flexibility and interpretability for downstream use.

## Technology Stack
- **Python** — core implementation language
- **TensorFlow / Keras** — model architecture, training, and serialization
- **NumPy** — numerical operations and tensor manipulation
- **Matplotlib** — visualization of training metrics and predictions
- **argparse** — structured command-line argument parsing

## Key Competencies Demonstrated
- Application of transfer learning to achieve strong performance with limited training data.
- Design of efficient image preprocessing and data-loading pipelines.
- Persistence and reuse of trained Keras models across environments.
- Translation of research-grade notebooks into deployable command-line tools.
- Disciplined Python project structure with clear separation of concerns.

## Acknowledgements

This project was completed as part of the **AI Programming with Python and TensorFlow Nanodegree**, delivered under the **Palestine Launch Pad Scholarship**, sponsored by **Google** and **Udacity**.
