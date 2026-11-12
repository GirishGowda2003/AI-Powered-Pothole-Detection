# AI-Powered-Pothole-Detection
# 🚧 AI-Powered Pothole Detection and Road Damage Reporting System

## 📌 Project Overview

The AI-Powered Pothole Detection and Road Damage Reporting System is a computer vision-based application designed to automatically identify potholes and road damage using images and videos.

The system uses YOLO (You Only Look Once) object detection to detect road damage, identify its location, and generate reports.

By integrating AI-based detection, GPS tracking, and interactive maps, the application aims to simplify road damage monitoring and support faster infrastructure maintenance.

## 🎯 Objectives

- Automatically detect potholes using AI.
- Identify road damage from images and videos.
- Display detected damage with bounding boxes.
- Capture GPS coordinates of damaged locations.
- Visualize road damage on an interactive map.
- Generate road damage reports for maintenance purposes.

## ✨ Key Features

- 🚗 Image-based pothole detection.
- 🎥 Video-based road damage detection.
- 🧠 YOLO-powered object detection.
- 📍 GPS-based location tracking.
- 🗺️ Interactive road damage map.
- 📊 Damage detection results and confidence scores.
- 📄 Automated road damage reporting.
- 🌐 User-friendly Streamlit interface.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Backend development |
| YOLO | Pothole and road damage detection |
| Ultralytics | YOLO model implementation |
| OpenCV | Image and video processing |
| NumPy | Numerical operations |
| Pillow | Image processing |
| Streamlit | Frontend application |
| FastAPI | Backend API |
| Supabase | Database and storage |
| Folium | Interactive map visualization |

## 🏗️ System Architecture

```text
             USER
               |
               v
       Streamlit Interface
               |
               v
        Upload Image/Video
               |
               v
        FastAPI Backend
               |
               v
        OpenCV Processing
               |
               v
        Pretrained YOLO Model
               |
               v
       Road Damage Detection
               |
               v
     Bounding Boxes + Confidence
               |
               v
        GPS Coordinates
               |
               v
       Supabase Database
               |
               v
      Interactive Map (Folium)
               |
               v
       Damage Report Generation
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
```

### 2. Navigate to the Project

```bash
cd pothole-detection
```

### 3. Create Virtual Environment

```bash
python -m venv venv
```

### 4. Activate Virtual Environment

Windows:

```bash
venv\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Download YOLO Model

Place your trained or pretrained pothole detection model inside the project directory.

Example:

```text
models/
    best.pt
```

### 7. Run the Application

```bash
streamlit run app.py
```

## 🔄 How the System Works

1. **Image/Video Upload:** Users upload road images or videos through the application.
2. **Image Processing:** OpenCV processes the uploaded media.
3. **AI Detection:** YOLO identifies potholes and other supported road damage categories.
4. **Damage Localization:** The system associates detected damage with GPS coordinates when location metadata or GPS data is available.
5. **Visualization:** Detected potholes are displayed with bounding boxes and confidence scores.
6. **Map Integration:** Road damage locations are displayed on an interactive map.
7. **Report Generation:** The system generates reports containing detected damage information and location details.

## 📊 Expected Output

- Original road image or video.
- Detected potholes with bounding boxes.
- Detection confidence scores.
- GPS coordinates, when available.
- Interactive road damage map.
- Road damage report.

## 🚀 Future Enhancements

- Real-time pothole detection using dashcam footage.
- Road damage severity classification.
- Automatic complaint submission to municipal authorities.
- Traffic-aware road damage monitoring.
- Multiple road damage category detection.
- Cloud-based deployment.
- Mobile application integration.
- AI-based road maintenance prioritization.

## 👨‍💻 Author

**Girish Gowda**

Computer Science Engineering | Data Science

Interested in Artificial Intelligence, Machine Learning, Deep Learning, and Computer Vision.

---

⭐ If you find this project interesting, consider giving the repository a star!
