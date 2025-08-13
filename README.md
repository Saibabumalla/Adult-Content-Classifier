# Adult-Content-Classifier

## Overview
**Adult-Content-Classifier** is a deep learning application that classifies images as **Adult Content (18+)** or **Normal Content**.  
It is designed for **content moderation**, **online safety**, and **ensuring a positive user experience** on various platforms.  

This project includes a **Streamlit** web app for quick testing and demonstrations, allowing users to upload images and get instant classification results.

---

## Features
- **Binary Classification**: Distinguishes between Adult (NSFW) and Normal images.
- **Streamlit Web Interface**: User-friendly, interactive, and browser-based.
- **Automatic Model Download**: Downloads the `nsfw_classifier.h5` model from cloud storage if missing locally.
- **Robust Preprocessing**: Handles corrupted or invalid image files gracefully.

---

## Tech Stack
- **Programming Language**: Python
- **Frameworks & Libraries**:
  - [Streamlit](https://streamlit.io/) – Web application framework
  - [TensorFlow / Keras](https://www.tensorflow.org/) – Deep learning model
  - [gdown](https://pypi.org/project/gdown/) – Google Drive file downloader
- **Dataset**: Custom dataset of labeled Adult and Normal content images

---

## Dataset
The dataset used for training the model can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1uY0FXh8dn4QBMK_g0-cgqASodXwc6Q_R?usp=drive_link).  
Alternatively, you can request access to the dataset by contacting the project author.

---

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/<your-username>/Adult-Content-Classifier.git
   cd Adult-Content-Classifier
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## Running the App Locally
Start the Streamlit application:
```bash
streamlit run app_adult.py
```

Then open the URL shown in the terminal (usually `http://localhost:8501`) in your browser.

---

## Model Download
The model file `nsfw_classifier.h5` is hosted on Google Drive.  
If it’s not found locally, it will be downloaded automatically when you start the app:
```python
import gdown

def download_model():
    url = "https://drive.google.com/file/d/1n3-mQzW4urQW-xypoNgky6bjy33NXeTp/view?usp=sharing"
    gdown.download(url, "nsfw_classifier.h5", quiet=False)
```

---

## Usage
1. Upload an image via the Streamlit interface.
2. The app will classify it as:
   - **Adult (NSFW)** – 18+ content detected
   - **Normal** – Safe content
3. View the classification result with confidence score.

---

## Results
- **Accuracy**: Achieved **94%** accuracy on the validation dataset.
- **Loss**: Training and validation loss curves indicate minimal overfitting.

---

## Screenshots


---

## Future Scope
- Extend to multi-class classification for various adult content categories.
- Implement real-time classification from webcam streams.
- Expand to video classification.

---

## Contributing
Contributions are welcome! Fork the repo, raise issues, or submit pull requests for improvements.

---

## Acknowledgments
- [TensorFlow / Keras Documentation](https://www.tensorflow.org/)
- [Streamlit Documentation](https://docs.streamlit.io/)

---

## Disclaimer
This tool is intended for **educational and research purposes** only.  
It should not be solely relied upon for production-level content moderation.


## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/<your-username>/Adult-Content-Classifier.git
   cd Adult-Content-Classifier
