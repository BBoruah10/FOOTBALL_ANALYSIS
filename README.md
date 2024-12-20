# ⚽ Football Analysis Using YOLO, OpenCV, and Python

## 🌟 Overview
Unleash the power of computer vision to analyze football plays like never before! This project uses YOLO (You Only Look Once), OpenCV, and Python to turn video footage into insightful data, tracking players, calculating speed, and measuring distances covered. Perfect for coaches, analysts, and football enthusiasts alike!

---

## ✨ Features
- 🔍 **Player Detection**: Real-time detection of football players using YOLO.
- 🎯 **Player Tracking**: Seamlessly track players across video frames.
- ⚡ **Speed and Distance Estimation**: Compute real-world metrics for player performance.
- 🎥 **Camera Movement Compensation**: Adjust player positions dynamically for accurate analysis.
- 🛠️ **Perspective Transformation**: Convert pixel data into real-world dimensions.
- 📊 **Visualization**: Stunning visual representations of player trajectories and statistics.

---

## 🛠️ Requirements
Ensure your environment is ready with these dependencies:

```bash
numpy<2               # Ensure compatibility with modules like OpenCV
opencv-python==4.7.0.68  # Stable version of OpenCV
ultralytics           # YOLO library (includes YOLOv8)
matplotlib            # For visualizing results
pandas                # For data manipulation (e.g., player stats, game events)
scipy                 # For scientific computations
torch>=1.9.0          # Required for YOLO models (PyTorch backend)
torchvision>=0.10.0   # For PyTorch image transformations
tqdm                  # For progress bars
seaborn               # For advanced visualizations
sklearn               # For clustering and additional data analysis
```

Install all requirements with:
```bash
pip install -r requirements.txt
```

---

## 🚀 Steps Involved

### **STEP 1: Object Detection**
- Leverage YOLO to detect players in video frames.
- Fine-tune the YOLO model using a football training dataset from [Roboflow](https://roboflow.com).

### **STEP 2: Player Tracking**
- Implement robust tracking algorithms to locate the bounding boxes of players across frames.

### **STEP 3: Annotation and Visualization**
- Draw ellipse-shaped bounding boxes for accurate player representation.
- Highlight ball acquisition events with clear annotations.

### **STEP 4: Player and Non-Player Clustering**
- Use K-Means clustering to differentiate players from non-players based on color.

### **STEP 5: Camera Movement Estimation**
- Estimate camera movement to:
  - Calculate accurate player distances.
  - Adjust player positions relative to camera shifts.

### **STEP 6: Perspective Transformation**
- Detect four pixel positions to create a trapezoid.
- Convert the trapezoid into a rectangle using known field dimensions.
- Map pixel coordinates into real-world coordinates for precise analysis.

### **STEP 7: Speed and Distance Estimation**
- Calculate speed and distance covered using real-world coordinates.

---

## 📂 Project Structure
```
football-analysis/
|
|-- data/                   # Training datasets and video footage
|-- models/                 # YOLO models and weights
|-- scripts/                # Python scripts for detection, tracking, and visualization
|-- results/                # Generated visualizations and reports
|-- requirements.txt        # Dependencies
|-- README.md               # Project documentation
```

---

## 🎥 Visualizations
- 🏃 Annotated video frames with player bounding boxes and trajectories.
- 📈 Statistical plots showcasing player speed, distance, and clustering analysis.
- 🔥 Heatmaps representing player movements on the field.

---

## 🏁 Getting Started
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/football-analysis.git
   cd football-analysis
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the analysis**:
   - Modify the `config.py` file to include your video file path and other parameters.
   - Execute the main script:
     ```bash
     python main.py
     ```

---

## 🤝 Contributing
We welcome contributions! Fork the repository, make improvements, and submit a pull request. Let's make football analysis even better together!

---

## 📜 License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## 🙌 Acknowledgments
- 🎓 [Roboflow](https://roboflow.com) for the football training dataset.
- 🤖 [YOLO](https://ultralytics.com/yolov8) for cutting-edge object detection.
- 🌍 OpenCV and the Python community for their invaluable tools and support.

---

⚽ **Dive into football analysis today and revolutionize the way you view the game!** 🚀

