# yolov7-pose-estimation

### Steps to Run Code

- **Clone the repository**:
  ```
  git clone https://github.com/Yzh-style/YoloV7_Fall_detection_Pose.git
  or
  git clone https://github.com/RizwanMunawar/yolov7-pose-estimation.git
  and replace file "pose-estimate.py" and "plots1" from this git folder
  ```
- **Go to the cloned folder**:

  ```bash
  cd YoloV7_Fall_detection_Pose
  ```
- **Create a virtual environment** (recommended):
  ```
  # Windows
  python3 -m venv Fall_detection_Pose
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  .\Fall_detection_Pose\Scripts\Activate.ps1
  ```
- **Upgrade pip**:
  ```bash
  pip install --upgrade pip
  ```
- **Install requirements**:
  ```bash
  pip install -r requirements.txt
  ```
- **Download YOLOv7 weights** and move to the working directory:
  [yolov7-w6-pose.pt](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-w6-pose.pt)

- **Run the code**:
  ```bash
  python pose-estimate.py

  # Options:
  python pose-estimate.py --source 0 --view-img  # For Webcam
  python pose-estimate.py --source 0 --view-img --blur  # Fro blur face function

  python pose-estimate.py --source "your-video.mp4" --device cpu  # For CPU
  python pose-estimate.py --source "rtsp://your-ip" --device 0 --view-img  # For LiveStream
  ```

- Output: The processed video will be saved as **your-file-keypoint.mp4**

### RESULTS

<img width="1764" height="669" alt="image" src="https://github.com/user-attachments/assets/a48f198d-e877-47ec-9ee1-30ced6e83646" />

### References
- YOLOv7 Repo: https://github.com/WongKinYiu/yolov7
- Ultralytics: https://github.com/ultralytics/yolov5

### 📖 Articles
- [YOLOv7 Training Guide](https://medium.com/augmented-startups/yolov7-training-on-custom-data-b86d23e6623)
- [Computer Vision Roadmap](https://medium.com/augmented-startups/roadmap-for-computer-vision-engineer-45167b94518c)
