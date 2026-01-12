# 🤟📷 Sign Language Recognition System (Computer Vision & Deep Learning)

## 📌 Overview
This project implements a **real-time Sign Language Recognition System** using **Computer Vision and Deep Learning**.  
It detects and classifies hand gestures representing **American Sign Language (ASL)** characters using a **Convolutional Neural Network (CNN)** and live webcam input.

The system is designed to bridge the communication gap by translating hand gestures into recognizable symbols through automated vision-based learning.

## 🎯 Project Objectives
- Capture hand gesture images using a webcam  
- Preprocess and standardize gesture data for model training  
- Train a CNN to classify multiple sign language gestures  
- Perform **real-time gesture recognition** using live video feed  


## 🧠 How the Project Works
1. **Hand Calibration**
   - A skin-color histogram is created using sample frames to isolate the hand region
   - This step improves segmentation accuracy under different lighting conditions  

2. **Data Collection**
   - Gesture images are captured using OpenCV
   - Images are converted to grayscale and resized to a fixed dimension
   - Data augmentation is applied using image flipping  

3. **Model Training**
   - A CNN model is trained on the prepared gesture dataset
   - The trained model is saved in `.h5` format for later inference  

4. **Real-Time Recognition**
   - Webcam feed is processed frame-by-frame
   - The trained CNN predicts the gesture shown in real time  


## 🛠️ Tech Stack
- **Programming Language:** Python  
- **Libraries & Frameworks:**  
  - OpenCV  
  - TensorFlow / Keras  
  - NumPy  
  - h5py  
- **Deep Learning Model:** Convolutional Neural Network (CNN)  
- **Environment:** Python 3.x  
- **Interface:** Webcam-based real-time recognition  


## 📂 Project Structure
- `set_hand_hist.py` → Creates hand histogram for segmentation  
- `create_gestures.py` → Captures gesture images for dataset creation  
- `load_images.py` → Loads and preprocesses gesture images  
- `cnn_model.py` → Defines and trains the CNN model  
- `recognize_gesture.py` → Performs real-time gesture recognition  
- `gestures/` → Stored gesture image datasets  
- `model/` → Saved trained CNN model  


## 📊 Dataset Details
- Multiple hand gesture classes representing ASL symbols  
- Each gesture contains thousands of grayscale images  
- Images are resized and normalized for consistent training  


## 🚀 Use Cases
- Assistive technology for hearing- and speech-impaired communication  
- Computer vision and deep learning learning project  
- Gesture-based human–computer interaction  
- Academic and portfolio demonstration of CNN-based image classification  


## 📌 Key Takeaways
- Demonstrates end-to-end application of computer vision and deep learning  
- Highlights real-time inference using trained neural networks  
- Shows practical challenges such as lighting variation and hand segmentation  


## 📎 Notes
This project focuses on gesture recognition at the character level and serves as a strong foundation for building more advanced sign language translation systems.
