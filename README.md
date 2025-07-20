
# 🎯 Face Detection and Recognition System

This project is a complete face detection and recognition system using **OpenCV**, **Haar Cascades**, and a deep learning model built with **Keras**. It captures images from an IP camera, detects faces, stores datasets, and performs real-time face recognition.

---

## 📌 Features

- 📸 Real-time face detection using IP webcam (`shot.jpg` stream)
- 🔍 Haar Cascade-based face detection
- 🗃️ Dataset creation (100 face samples per person)
- 🧠 Face recognition using a trained CNN model (`final_model.h5`)
- 💾 Saves processed images and labels using `pickle`
- 📊 Live prediction with name display on frame

---

## 🛠️ Technologies

- Python
- OpenCV
- NumPy
- Keras (TensorFlow backend)
- Haar Cascades
- IP Webcam
- Pickle

---

## 📂 Project Structure
face-recognition/
├── face_collection.py # Collects face data from IP camera
├── data_preparation.py # Converts images to grayscale & pickles data
├── face_recognition_live.py # Real-time face recognition
├── final_model.h5 # Trained model for prediction
├── haarcascade_frontalface_default.xml
├── images/ # Captured face samples
└── cleandata/ # Pickled image & label data


---

## 🚀 How to Use

1. **Capture Face Data**
   - Run `face_collection.py`
   - Collect 100 samples per person
   - Press `q` to exit

2. **Preprocess and Save Data**
   - Run `data_preparation.py` to convert, resize, and save face data

3. **Train the Model**
   - (Add a training script separately if needed)

4. **Live Prediction**
   - Run `face_recognition_live.py`
   - The model predicts and displays the name live
   - Press `q` to quit

---

## ✅ Notes

- Update your **IP camera URL** (e.g., `http://192.168.xx.xx:8080/shot.jpg`)
- Adjust paths for Haar Cascade XML and model as needed
- Images must be in grayscale and 100x100 size for prediction

---

## 🔮 Future Improvements

- Add GUI interface (Tkinter/PyQt)
- Expand dataset with more users
- Implement local webcam/video file input
- Add attendance logging

---

Made with by Alok using OpenCV & Deep Learning.


