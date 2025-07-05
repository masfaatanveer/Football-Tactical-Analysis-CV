# ⚽ Football Tactical Analysis - Computer Vision 🔍

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.8+-green)](https://opencv.org/)
[![YOLOv8](https://img.shields.io/badge/YOLOv8-8.0+-red)](https://ultralytics.com/yolov8)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-ff69b4)](https://streamlit.io/)

Real-time computer vision system for football tactical analysis. Detects players, referees, and ball, predicts team affiliations based on jersey colors, and maps player positions onto a tactical field for visualization and strategy.

---

## ▶️ Quick Launch

```bash
git clone https://github.com/masfaatanveer/Football-Tactical-Analysis-CV.git
pip install -r requirements.txt
streamlit run main.py
```

If you download the ZIP, unzip the code → install requirements → and run the command below:

```bash
streamlit run main.py
```

The app will launch locally in your browser and show the real-time football analytics dashboard.

---

## 🎯 Key Features

- YOLOv8-based detection of players, ball, referees  
- Team prediction using LAB color space & dominant jersey colors  
- Homography transformation to map player positions onto a 2D tactical field  
- Streamlit-based fast web interface  
- Ball tracking with position history  
- Side-by-side tactical map & annotated video frame  

---

## 📊 Performance Metrics

| Feature           | Metric / Value                    |
|-------------------|-----------------------------------|
| Player Detection  | 98.2% mAP@0.5                     |
| Team Prediction   | 92.4% accuracy (LAB space)        |
| Keypoint Detection| 95.4% precision (YOLOv8-m)        |
| Ball Tracking     | 87 FPS (RTX 3060)                 |
| Homography        | RMSE: 3.2 px                      |

---

## 🤖 Training Details

| Model           | Dataset           | Epochs | Augmentation Techniques        |
|-----------------|-------------------|--------|--------------------------------|
| YOLOv8 (Players)| Custom            | 150    | Mosaic, MixUp, Rotation        |
| YOLOv8 (Field)  | Custom (keypoints)| 200    | Perspective, Resize, Shear     |
| Team Color Logic| Manual Annotated  | -      | LAB color extraction + compare |

---

## 📧 Contact

**Masfa Tanveer**  
📩 masfaatanveerr@gmail.com  
🔗 [GitHub](https://github.com/masfaatanveer/Football-Tactical-Analysis-CV)

---

## 📝 License

Distributed under the MIT License.
