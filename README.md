This project aims to detect and classify traffic signs using the YOLOv5 object detection algorithm. The YOLO (You Only Look Once) algorithm is a real-time object detection system that achieves high accuracy and efficiency.

yolo v5 link - https://github.com/ultralytics/yolov5
dataset link - https://www.kaggle.com/datasets/valentynsichkar/traffic-signs-dataset-in-yolo-format
## Dataset

To train the YOLOv5 model, we utilized a custom dataset specifically collected and labeled for traffic sign detection. The dataset includes a variety of traffic sign images captured from different environments, angles, and lighting conditions. Unfortunately, I don't have access to specific dataset links as my training only goes up until September 2021. However, you can find various public traffic sign datasets online, such as the German Traffic Sign Recognition Benchmark (GTSRB) dataset.

## Getting Started

To run this project on your local machine, follow these steps:

1. Clone the repository: `git clone https://github.com/your-repo.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Download the pre-trained YOLOv5 model weights: [YOLOv5](https://link-to-yolov5-weights)
4. Load the dataset and preprocess it according to the project requirements.
5. Train the YOLOv5 model using the prepared dataset.
6. Test the trained model on new images or videos.

## Usage

Here are the basic commands to train and test the YOLOv5 model:

- Training:
  
  python train.py --data data.yaml --cfg models/yolov5s.yaml --weights yolov5s.pt
  

- Testing:
  
  python detect.py --source test_images/ --weights runs/train/exp/weights/best.pt --conf 0.4
  
