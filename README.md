# Fingerprinting AI-Generated Images

This repository investigates whether **AI image generation models leave identifiable fingerprints** in the images they produce. The objective is to determine if low-level patterns can be used to **attribute an image to its source model**, rather than simply classifying images as real or AI-generated.

This project is an early-stage academic research prototype.

## Current Status
- 3 AI image generation models
- 15 images per model
- Initial experiments completed
- Single executable Python script

## Motivation
As AI-generated images become widespread, identifying **which model generated an image** is important for:
- AI content attribution
- Deepfake and misinformation analysis
- Digital forensics
- Trust and safety research

This work focuses on **model-specific artifacts** instead of visual or semantic content.

## Methodology
The approach followed in this project:
1. Load AI-generated images from different models
2. Extract low-level statistical and frequency-based features
3. Train a classifier to distinguish between generation models
4. Evaluate whether model-specific patterns persist across samples

The emphasis is on **AI model fingerprinting**, not binary AI detection.

## Repository Contents
.
├── ai_image_classifier.py # Main experiment script (exported from Google Colab)
└── README.md


## Requirements
- Python 3.9 or higher
- NumPy
- OpenCV
- scikit-learn
- TensorFlow or PyTorch (as used in the script)

## Usage

Run the experiment using:
python ai_image_classifier.py

All preprocessing, feature extraction, training, and evaluation steps are contained within this script.

## Limitations

Scaling the dataset to hundreds of images per model

Adding advanced texture descriptors (GLCM, wavelets)

Comparing handcrafted features with CLIP embeddings

Evaluating generalization to unseen prompts and models

Exploring robustness against post-processing and compression

Motivation

This project is intended as a foundation for research in:

AI model attribution

Trustworthy and interpretable machine learning

Forensic analysis of generative models

It is designed to be lightweight, explainable, and reproducible.

Author

Sujeeth Sukumar
MS in Data Science
University of Maryland, College Park
Email: sujeeth@umd.edu
