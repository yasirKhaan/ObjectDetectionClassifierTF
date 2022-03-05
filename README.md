# ObjectDetectionClassifierTF


# Yolo v3 Object Detection with Tensorflow 2.0
Yolo v3 is an algorithm that uses deep convolutional neural networks to detect objects. <br> <br>

## Getting started

### Prerequisites
This project is written in Python 3.7 using Tensorflow 2.0 (deep learning), NumPy (numerical computing), Pillow (image processing), OpenCV (computer vision) and seaborn (visualization) packages.

```
pip install -r requirements.txt
```


```
python load_weights.py
```

## Running the model
You can run the model using `detect.py` script. The script works on images, video or your webcam. Don't forget to set the IoU (Intersection over Union) and confidence thresholds.
### Usage
```
python detect.py <images/video/webcam> <iou threshold> <confidence threshold> <filenames>
```
### Images example
Let's run an example using sample images.
```
python detect.py images 0.5 0.5 data/images/dog.jpg data/images/office.jpg
```
Then you can find the detections in the `detections` folder.
<br>
You should see something like this.

### Video example
You can also run the script with video files.
```
python detect.py video 0.5 0.5 data/video/shinjuku.mp4
```
The detections will be saved as `detections.mp4` file.

### Webcam example
The script can also be ran using your laptops webcam as the input. Example command shown below.
```
python detect.py webcam 0.5 0.5
```
The detections will be saved as 'detections.mp4' in the data/detections folder.

