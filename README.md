#  Video Forgery Detection using Deep Neural Networks (DNN)

##  Project Overview

In the modern digital era, videos play a vital role in information sharing, journalism, and entertainment. However, with the rapid advancement of editing tools and AI-based generation methods, video forgery has become increasingly sophisticated and difficult to detect. This project, **Video Forgery Detection using DNN (Deep Neural Networks)**, focuses on developing an intelligent system that can automatically detect forged (fake) frames in a video sequence using deep learning techniques.

The proposed system utilizes **Convolutional Neural Networks (CNN)** for spatial feature extraction and **Gated Recurrent Units (GRU)** for learning temporal dependencies in video frames. CNNs effectively capture texture, edge, and motion-based inconsistencies, while GRU layers model the sequential nature of video data, enabling the model to distinguish between real and manipulated content with high accuracy. The system combines both spatial and temporal information, providing a powerful hybrid DNN-based architecture for forgery detection.

The project includes a **Tkinter-based graphical user interface (GUI)** that allows users to:

* Upload a dataset of real and forged videos
* Automatically extract and normalize video frames
* Train the DNN model
* Evaluate model performance using accuracy, precision, recall, and F1-score metrics
* Detect forgery in new videos by visualizing real vs. forged frames in real time

During prediction, the system processes each video frame, classifies it as real or forged, and displays the results dynamically. It also generates a new output video with forged frames removed, ensuring visual clarity of genuine content.

This tool can be beneficial for **digital forensics**, **media verification**, **deepfake detection**, and **academic research**. Built using Python, TensorFlow, Keras, OpenCV, and scikit-learn, it demonstrates the power of machine learning in combating misinformation and enhancing digital trust.

Overall, this project bridges the gap between deep learning research and real-world video forensics, offering a robust and user-friendly solution for automated video forgery detection.

---

##  Technologies Used

* **Python 3.8+**
* **TensorFlow / Keras**
* **OpenCV**
* **NumPy & Pandas**
* **Scikit-learn**
* **Tkinter (GUI framework)**
* **Matplotlib**

---

## 📂 Project Structure

```
VideoForgeryDetection/
│
├── video_forgery_detection.py      # Main application with GUI and DNN model
├── model/                          # Saved model weights, datasets, and history
├── testVideos/                     # Test video samples (optional)
├── README.md                       # Project documentation
└── requirements.txt                # List of dependencies
```

---

## 🖥️ Installation & Setup

1. **Clone this repository**

   ```bash
   git clone https://github.com/1510ritika/VideoForgeryDetection.git
   cd VideoForgeryDetection
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **(Optional)** Create a `model/` directory if it doesn’t exist

   ```bash
   mkdir model
   ```

4. **Run the application**

   ```bash
   python video_forgery_detection.py
   ```

---

##  How to Use

1. Launch the program using the Tkinter GUI.
2. Click **“Upload Video Dataset”** to load your folder containing *real* and *forged* videos.
3. Click **“Shuffle & Normalize Video Frames”** to preprocess the dataset.
4. Split the data using **“Split Frames Train & Test”**.
5. Train your DNN model using **“Train DNN Model”** (weights are saved automatically).
6. Finally, click **“Video Based Forgery Detection”** to test your own video.
7. The system will highlight forged frames in real time and save a “cleaned” version of the video.

---

##  Evaluation Metrics

* **Accuracy**
* **Precision**
* **Recall**
* **F1-Score**

These metrics are computed after testing to evaluate model performance on unseen videos.

---

##  Acknowledgements

This project demonstrates the integration of deep learning and computer vision for digital media forensics. Special thanks to the open-source community and research papers that inspired the implementation of DNN architectures for video-based forgery detection.

---

Would you like me to also create a `requirements.txt` file listing all the necessary Python libraries for this project (so it installs easily on any computer)?
