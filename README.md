# 🚦 Traffic Management System

## 📌 Overview
The **Traffic Management System** is an AI-based project that utilizes **YOLOv8** for real-time vehicle detection and dynamically adjusts traffic light timings based on vehicle density. This system enhances traffic efficiency by allocating green light durations based on actual traffic conditions.

## ✨ Features
- 🚗 **Real-time vehicle detection** (cars, buses, trucks, motorbikes)
- ⏳ **Dynamic traffic light control** based on vehicle count
- 🚦 **Lane filtering** to ensure correct detection
- 📊 **Traffic data logging** for further analysis
- 🖼️ **Works with static images** instead of video input

## 🛠️ Project Structure
```
Traffic-Management-System/
│── main.py                 # Main script to run the project
│── config.py               # Configuration file for parameters
│── vehicle_detector.py     # Module for vehicle detection
│── lane_detector.py        # Module for lane detection
│── traffic_analyzer.py     # Module for traffic analysis
│── utils.py                # Utility functions (visualization, logging)
│── requirements.txt        # List of dependencies
│── README.md               # Documentation
```

## 🚀 Installation & Setup
### 1️⃣ Clone the Repository
```bash
https://github.com/sauravranjann/Traffic_management_system_yolov8m.git
cd Traffic_management_system_yolov8m
```
### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
### 3️⃣ Configure `config.py`
Modify the **image paths** in `config.py` to match your dataset:
```python
IMAGE_PATHS = [
    "C:\\Users\\Lenovo\\Downloads\\1651869427801first.png",
    "C:\\Users\\Lenovo\\Downloads\\image22.jpg",
    "C:\\Users\\Lenovo\\Downloads\\image3.jpg",
    "C:\\Users\\Lenovo\\Downloads\\images4.jpeg"
]
```

### 4️⃣ Run the Project
```bash
main.py
```

## 📷 Sample Output
When the script runs, it detects vehicles in the images and calculates the **optimal green time**:
```
0: 640x384 14 cars, 2 buses, 3 trucks, 83.5ms
Speed: 6.0ms preprocess, 83.5ms inference, 2.0ms postprocess
```
🖼️ Output Images
    ![image](https://github.com/user-attachments/assets/9aee43eb-4f86-4335-8640-d6c89b6284a7)




## 🛠️ Customization
- 🏎 **Change the YOLO model** in `config.py`:
  ```python
  MODEL_PATH = "yolov8m.pt"  # Use a larger model for better accuracy
  ```
- 🔧 **Adjust traffic light timing**:
  ```python
  BASE_GREEN_TIME = 10  # Base green time in seconds
  MAX_GREEN_TIME = 60   # Max green time limit
  TIME_INCREMENT = {"car": 2, "bus": 2, "truck": 2, "motorbike": 1}
  ```

## 🤖 Tech Stack
- **Python** 🐍
- **YOLOv8 (Ultralytics)** 🖼️
- **OpenCV** 👁️
- **NumPy** 🔢

## 📜 License
This project is **open-source** under the [MIT License](LICENSE).

## 🙌 Contributing
1. **Fork** the repo.
2. **Create a branch** for your feature (`git checkout -b feature-name`).
3. **Commit changes** (`git commit -m "Added new feature"`).
4. **Push to GitHub** and create a Pull Request.

## 📧 Contact
For queries or suggestions, feel free to reach out:
📩 Email: [amarana5006@gmail.com](mailto:amarana5006@gmail.com)  
GitHub: [Amanrana1](https://github.com/Amanrana1)  

---
🚀 **Let's make traffic management smarter!**

#   T r a f f i c _ l i g h t _ m a n a g e m e n t _ s y s t e m _ u s i n g _ a i 
 
 