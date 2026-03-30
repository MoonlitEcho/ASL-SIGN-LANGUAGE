# 🤟 ASL Sign Language Recognition

A real-time American Sign Language (ASL) alphabet recognition system using a Convolutional Neural Network (CNN) trained on hand gesture images.

---

## 📁 Repository Structure

| File | Description |
|------|-------------|
| `Alphabet.jpg` | Reference image of the ASL alphabet chart |
| `cnn8grps_rad1_model.h5` | Pre-trained CNN model (8 gesture groups) |
| `data_collection_binary.py` | Collect binary/thresholded hand gesture images for training |
| `data_collection_final.py` | Final data collection pipeline with preprocessing |
| `final_pred.py` | Real-time prediction script using the trained model |
| `white.jpg` | Blank white background used during image preprocessing |

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install tensorflow keras opencv-python numpy
```

### Run Real-Time Prediction
```bash
python final_pred.py
```

The script will:
1. Capture live video from your webcam
2. Detect and isolate the hand region
3. Preprocess the image (binarization, background removal)
4. Predict the ASL letter using the CNN model
5. Display the result on screen

### Collect Training Data
```bash
python data_collection_final.py
```

---

## 🛠️ Tech Stack

- **Python** — Core language
- **OpenCV** — Real-time video capture and image processing
- **TensorFlow / Keras** — CNN model training and inference
- **NumPy** — Numerical operations

---

## 📌 Future Improvements

- [ ] Extend to full ASL vocabulary (words & phrases)
- [ ] Add dynamic gesture support (letters like J and Z)
- [ ] Deploy as a web app using Streamlit or Flask
- [ ] Integrate text-to-speech output

---
