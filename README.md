# Parking space count
This project uses a YOLOv8-trained model to count the available parking space. It further showcases how we can use OpenVINO for faster inference.

The dataset to train the model was downloaded from Roboflow.


### Requirements:

- ultralytics==8.0.131
- torch==1.13.0
- opencv-python==4.8.0.74
- openvino-dev==2023.0.0


### Steps to run:

1. Download the dataset from [here](https://public.roboflow.com/object-detection/pklot)
2. Use the file `1.datasplit.py` to split the dataset (optional)
3. Create a `data.yaml` file and run `2.yv8_train.py` to start training
4. A model will be created at `./runs/detect/yolov8n_park_20e/weights` with the name `best.pt`
5. Run the file `YOLOv8-challenge-2.ipynb` for inferencing


### References:

[OpenVINO](https://docs.openvino.ai/2023.0/home.html)
[Blog](https://learnopencv.com/train-yolov8-on-custom-dataset/)
[SO](https://stackoverflow.com/questions/75324341/yolov8-get-predicted-bounding-box)
