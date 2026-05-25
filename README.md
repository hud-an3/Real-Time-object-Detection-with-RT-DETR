# RT-DETR Object Detection and Benchmarking

This project demonstrates real-time object detection using the RT-DETR (Real-Time Detection Transformer) model. The notebook includes model setup, COCO dataset preparation, pretrained weight loading, image inference, video detection, and benchmarking against YOLOv8.

---

## Features

* RT-DETR model inference using pretrained weights
* COCO dataset integration
* Real-time image object detection
* Video object detection pipeline
* RT-DETR vs YOLOv8 speed comparison
* Visualization of detections and benchmark results
* Threshold sensitivity analysis

---

## Technologies Used

* Python
* PyTorch
* Ultralytics
* OpenCV
* NumPy
* Matplotlib
* COCO Dataset

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/RT-DETR-Object-Detection.git
cd RT-DETR-Object-Detection
```

Install dependencies:

```bash
pip install ultralytics supervision requests torch torchvision opencv-python matplotlib numpy imageio gdown
```

---

## Dataset

This project uses the COCO 2017 validation dataset.

Dataset files are automatically downloaded inside the notebook using:

```python
wget http://images.cocodataset.org/zips/val2017.zip
wget http://images.cocodataset.org/annotations/annotations_trainval2017.zip
```

---

## Model Used

The project uses:

* RT-DETR-L
* RT-DETR-R50 pretrained weights
* YOLOv8-L for benchmarking comparison

---

## Results

The notebook demonstrates:

* Object detection on sample images
* Detection on videos
* Benchmark comparison between RT-DETR and YOLOv8
* Performance visualization graphs

---

## Example Tasks Performed

### Image Detection

The model detects multiple objects from sample images such as:

* People
* Vehicles
* Animals
* Everyday objects

### Video Detection

The project also performs frame-by-frame object detection on videos using OpenCV.

### Benchmarking

The notebook compares:

* Inference speed
* Detection sensitivity
* Number of predicted bounding boxes
* Threshold stability

---

## Future Improvements

* Fine-tuning RT-DETR on custom datasets
* Real-time webcam detection
* Deployment using FastAPI or Streamlit
* TensorRT optimization for faster inference
* Edge deployment on embedded devices

