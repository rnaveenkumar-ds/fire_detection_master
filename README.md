# 🔥 Forest Fire & Smoke Detection System using Deep Learning

## 📌 Project Overview

This project is a Deep Learning based Forest Fire and Smoke Detection System developed using TensorFlow, Keras, OpenCV, and Transfer Learning with EfficientNetB0.

The system can:

- Detect Fire 🔥
- Detect Smoke 🌫️
- Perform Real-Time Webcam Detection
- Generate Accuracy & Loss Graphs
- Create Confusion Matrix
- Produce Classification Reports

This project uses a Kaggle dataset and Transfer Learning to achieve high classification accuracy.

---

# 🎯 Objectives

The main objectives of this project are:

- Early forest fire detection
- Smoke detection using CNNs
- Real-time monitoring using webcam
- Reduce wildfire damage
- Build an AI-based surveillance system

---

# 🧠 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| TensorFlow | Deep Learning Framework |
| Keras | Model Building |
| OpenCV | Real-Time Detection |
| EfficientNetB0 | Transfer Learning Model |
| Matplotlib | Visualization |
| Seaborn | Confusion Matrix |
| Scikit-Learn | Evaluation Metrics |
| KaggleHub | Dataset Download |

---

# 📂 Dataset Information

## Dataset Used

Dataset Name:
Forest Fire Dataset

Dataset Source:

:contentReference[oaicite:0]{index=0}

---

# 📁 Dataset Structure

```text
forest-fire/
│
├── train_fire/
├── train_smoke/
├── test_small/
└── test_big/
```

---

# ⚠ Important Dataset Observation

The dataset contains:

- Fire Images
- Smoke Images

But it DOES NOT contain:

- Normal forest images
- Background scenes
- Non-fire images

This means the model only learns:

- Fire
- Smoke

And not:

- Normal objects
- Trees
- Sunlight
- Clouds
- Roads

So real-world accuracy may decrease in practical environments.

---

# ✅ Suggested Improvement

Add another class:

```text
non_fire/
```

Include:

- Forest images
- Rivers
- Mountains
- Roads
- Empty landscapes
- Sunlight scenes

Then train using:

```python
classes = [
    "fire",
    "smoke",
    "non_fire"
]
```

This significantly improves real-world performance.

---

# 🏗 Project Architecture

```text
Input Image
      ↓
Data Preprocessing
      ↓
Data Augmentation
      ↓
EfficientNetB0
      ↓
Dense Layers
      ↓
Softmax Classification
      ↓
Prediction Output
```

---

# 🖼 Sample Output Classes

| Class | Meaning |
|---|---|
| Fire | Forest Fire Detected |
| Smoke | Smoke Detected |

---

# 🧹 Data Preprocessing

The following preprocessing techniques are used:

- Image Resizing
- Normalization
- Data Augmentation
- Horizontal Flip
- Rotation
- Zoom
- Width Shift
- Height Shift

---

# 🧠 Deep Learning Model

## Transfer Learning Model

EfficientNetB0 is used as the base model.

Advantages:

- Lightweight
- High Accuracy
- Faster Training
- Good Feature Extraction
- State-of-the-Art Performance

---

# ⚙ Model Configuration

```python
IMG_SIZE = 224
BATCH_SIZE = 32
EPOCHS = 15
LEARNING_RATE = 0.0001
```

---

# 📊 Evaluation Metrics

The project evaluates:

- Accuracy
- Loss
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

# 📈 Accuracy Graph

The project generates:

- Training Accuracy Graph
- Validation Accuracy Graph

These graphs help analyze:

- Overfitting
- Underfitting
- Training Stability

---

# 📉 Loss Graph

The project also generates:

- Training Loss Graph
- Validation Loss Graph

This helps measure model convergence.

---

# 🔲 Confusion Matrix

The confusion matrix visualizes:

- Correct Predictions
- Incorrect Predictions

Example:

```text
                 Predicted
               Fire  Smoke

Actual Fire      95     5
Actual Smoke      7    93
```

---

# 📋 Classification Report

The classification report includes:

- Precision
- Recall
- F1-Score
- Support

Example:

```text
              precision    recall    f1-score

fire            0.95       0.94       0.94
smoke           0.94       0.95       0.94
```

---

# 💻 Real-Time Detection

The system uses OpenCV for webcam detection.

Features:

- Real-Time Prediction
- Live Webcam Feed
- Confidence Score
- Dynamic Labels

Example Output:

```text
fire : 98.22%
```

or

```text
smoke : 95.10%
```

---

# 🧪 Installation

## Step 1: Clone Repository

```bash
git clone <repository_link>
cd forest-fire-detection
```

---

# 📦 Install Dependencies

```bash
pip install tensorflow
pip install opencv-python
pip install matplotlib
pip install seaborn
pip install scikit-learn
pip install kagglehub
pip install pandas
```

---

# ▶ Run Project

```bash
python main.py
---

---

# 💾 Saved Model

The trained model is saved as:

```text
final_forest_fire_model.h5
```

This model can later be:

- Deployed
- Converted into API
- Used in Streamlit
- Used in Mobile Apps

---

# 🚀 Future Improvements

Future enhancements include:

## 1. Non-Fire Class

Add background scenes.

---

## 2. YOLOv8 Detection

Instead of classification:

- Detect exact fire location
- Draw bounding boxes

---

## 3. Smoke + Fire Combined Detection

Multi-class object detection.

---

## 4. Email Alert System

Send alerts when fire is detected.

---

## 5. Telegram Notification

Real-time mobile alerts.

---

## 6. Streamlit Dashboard

Interactive web interface.

---

## 7. Cloud Deployment

Deploy using:

- AWS
- Azure
- Google Cloud

---

## 8. Drone Surveillance

Use drone cameras for wildfire monitoring.

---

# 📌 Applications

This system can be used in:

- Forest Surveillance
- Wildlife Protection
- Industrial Safety
- Smart Cities
- Disaster Management
- Environmental Monitoring

---

# ⚠ Limitations

Current limitations:

- No non-fire class
- May misclassify sunlight
- Limited dataset diversity
- Classification only
- Not object localization

---

# 🎓 Learning Outcomes

Through this project, the following concepts are learned:

- Deep Learning
- CNNs
- Transfer Learning
- Image Classification
- TensorFlow
- OpenCV
- Data Augmentation
- Model Evaluation
- Real-Time Detection

---

# 🏁 Conclusion

This project demonstrates how Deep Learning can be used for Forest Fire and Smoke Detection using Transfer Learning and Real-Time Webcam Monitoring.

The project successfully:

- Detects Fire
- Detects Smoke
- Performs Real-Time Classification
- Uses EfficientNetB0 for high accuracy

Although the current dataset has limitations, the project forms a strong foundation for advanced wildfire monitoring systems.

---

# 👨‍💻 Author

Name: Your Name

Domain:
Data Science | AI/ML | Deep Learning

---

# 📜 License

This project is for educational and research purposes.

---
