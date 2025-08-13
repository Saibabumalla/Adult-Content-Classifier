# Adult-Content-Classifier

## Overview
**Adult-Content-Classifier** is a deep learning project that classifies images as **Adult Content (18+)** or **Normal Content**.  
It’s built to support **content moderation**, **online safety**, and **compliance** by detecting NSFW (Not Safe For Work) material before it’s displayed.

The project includes a **Streamlit** web app that allows you to upload images and get instant classification results.

---

## Features
- **Binary Classification** – Detects `Adult (NSFW)` vs `Normal` images.
- **Streamlit Web App** – Clean, interactive interface.
- **Automatic Model Download** – Model is fetched from cloud storage if missing locally.
- **Invalid Image Handling** – Skips corrupted or unreadable files.

---

## Tech Stack
- **Language:** Python
- **Frameworks/Libraries:**
  - [Streamlit](https://streamlit.io/)
  - [TensorFlow / Keras](https://www.tensorflow.org/)
  - [gdown](https://pypi.org/project/gdown/)
- **Model:** Pre-trained `.h5` binary classifier
- **Dataset:** Custom dataset with labeled Adult and Normal images

---

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/<your-username>/Adult-Content-Classifier.git
   cd Adult-Content-Classifier
