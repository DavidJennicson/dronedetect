### YOLOv9 Object Detection Readme

This Python script demonstrates real-time object detection using YOLOv9 (You Only Look Once version 9) with the Ultralytics library. YOLO is an efficient real-time object detection algorithm, and YOLOv9 represents the latest version of the YOLO series.

#### Prerequisites

- Python 3.x installed on your system
- Required libraries: Ultralytics

#### Installation

To use this script, you need to install the Ultralytics library. You can install it via pip:

```bash
pip install ultralytics
```

#### Usage

1. Clone or download the script to your local machine.
2. Ensure that you have the model weights file `best.pt` in the same directory as the script.
3. Run the script using Python:

```bash
python yolo_v9_detection.py
```

#### Script Explanation

- The `ModelType` enum specifies the type of YOLO model to use. Currently, only the `BEST` model is supported, which corresponds to the `best.pt` weights file.
- The `Camera` enum specifies the input source for object detection. In this script, it's set to `LAPTOP`, indicating the laptop's webcam.
- The `liveObjDetection` function initializes the YOLO model with the specified model type and performs real-time object detection using the webcam feed.
- To change the input source or use a different model type, modify the function parameters accordingly.
- When you run the script, it will open a window showing the webcam feed with real-time object detection bounding boxes drawn around detected objects.

#### Additional Notes

- You can customize the script further to use different YOLOv9 model versions or input sources by modifying the `ModelType` and `Camera` enums accordingly.
- Ensure that you have appropriate permissions to access the webcam if you're using a camera as the input source.
- For more advanced usage and configuration options, refer to the Ultralytics library documentation.

