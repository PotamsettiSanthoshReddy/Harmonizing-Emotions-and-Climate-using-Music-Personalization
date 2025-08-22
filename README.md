# 🎶 Harmonizing Emotions and Climate through Personalized Music 🎶

## 👥 Contributors  
- **Santhosh Reddy**  
  GitHub: [PotamsettiSanthoshReddy](https://github.com/PotamsettiSanthoshReddy)

---

## 🌟 Abstract

This project introduces an intelligent, cloud-powered music recommendation system that adapts to both your **emotional state** and **current weather conditions**. By combining **facial emotion recognition** and **environmental analysis**, it delivers a uniquely tailored music experience in real-time.  

Utilizing webcam-based emotion detection and weather recognition (sunny, rainy, cloudy, etc.), the system integrates with platforms like **Spotify** to recommend songs that match or enhance your mood. The overall goal is to offer a context-aware, emotionally intelligent listening experience powered by cloud services and machine learning.

---

## 📌 Project Overview

This application blends **computer vision**, **machine learning**, and **cloud integration** to personalize music using:

### 🎭 Emotion Detection
- The user's facial image is captured via webcam using **OpenCV**.
- A combination of **CNN** and **DNN** models predicts emotional states like:
  - Happy
  - Sad
  - Angry
  - Surprised
  - Fearful
  - Neutral
- The trained model (`final_model.h5`) can be updated or fine-tuned using the `Emotion_detector_version2` notebook.

### 🌤️ Weather Detection
- Environmental analysis is performed using visual input from the webcam.
- The system predicts the weather conditions (e.g., sunny, rainy, cloudy) to complement emotional insights.

### 🎵 Music Recommendation
- Over **160,000 songs** (retrieved via the **Spotify Web API**) are used to train a **K-Means clustering** model.
- Songs are categorized into:
  - **Class 0:** Very Entertaining
  - **Class 1:** Relaxing
- Based on emotion and weather:
  - If the user is **sad**, the system suggests **uplifting** tracks.
  - If the user is **happy**, more **relaxing** songs are recommended to maintain balance.

---

## 📊 Dataset

- The dataset includes metadata like **artist**, **year**, **genre**, and **popularity**, aiding accurate clustering.
- Real-time webcam inputs (emotion + weather) fine-tune the song suggestions, creating a more responsive and personalized experience.

---

## 🛠️ Libraries & Tools Used

- **OpenCV**
- **TensorFlow**
- **Keras**
- **Sklearn**
- **LightGBM**
- **Spotipy (Spotify API)**
- **Tkinter (GUI)**
- **Pillow**
- **NumPy**

---

## 🚀 How to Run

1. Clone the repository and navigate to the project directory.
2. Run the main script:  
   ```bash  
   python run.py  
   ```
3. A GUI window will launch prompting you to begin emotion detection.
4. The webcam will capture your image and perform:
   - **Facial emotion recognition**
   - **Weather condition analysis**
5. Based on this combined data, **personalized Telugu songs** will be recommended.
6. Songs will open automatically on **Spotify**.
7. To exit webcam mode, press **`q`**.

🎧 Enjoy a music experience tailored to your mood and your surroundings!
