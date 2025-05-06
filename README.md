
# 🎵 Emotion-Based Music Recommender

This Streamlit web app detects your emotion in real-time using your webcam and recommends songs based on your mood, selected language, and favorite singer. It uses deep learning, MediaPipe for facial/hand landmark detection, and YouTube for dynamic music recommendations.



> Emotion is captured from your face and hand landmarks in real-time. Once detected, a search query is generated like:
> ```
> [language] + [emotion] + song + [singer]
> ```
> and opened on YouTube automatically!

---

## 🧠 Features

- Real-time emotion detection using webcam
- Facial and hand landmark tracking via **MediaPipe**
- Emotion classification using a pre-trained **Keras** model
- Dynamic music recommendations via **YouTube**
- Easy-to-use interface with **Streamlit**

---

## 📝 Usage

1. Enter your **preferred language** and **singer** name.
2. Let the webcam **detect your emotion**.
3. Click **"Recommend me songs"**.
4. YouTube will open with emotion-based search results.

---

## 🧾 Requirements

See [requirements.txt](./requirements.txt)

> Packages used:
> - `streamlit`
> - `streamlit-webrtc`
> - `mediapipe`
> - `opencv-python`
> - `keras`
> - `numpy`
> - `av`

---

## 🛠️ Model Details

- The emotion recognition model (`model.h5`) takes normalized landmark coordinates and classifies into predefined emotions.
- Emotion labels are loaded from `labels.npy`.

---

## 🙋‍♀️ Contributors

- [Diwakar Mahotra](https://github.com/CD-Coder-Diwakar)


## 💡 Future Improvements

- Add multi-language support for UI
- Enhance emotion prediction using more robust models
- Integrate music streaming services (e.g., Spotify API)
