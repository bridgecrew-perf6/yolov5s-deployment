# YOLOv5 custom dataset (Easy Guide)

Please use this on google colab environment. Also, the provided notebook is using mask detector as the example dataset <br/>
You can find the available dataset at [here](https://universe.roboflow.com/) <br/>
This example is using the URL download link, which will download the data into temporary repository in google colab (won't consume google drive space)

# Three main steps and you're good to go
- Setup Environment
- Training Process
- Testing the model

## Setup Environment
- Create temporary yolov5 repository that is cloned from [here](https://github.com/ultralytics/yolov5)
- Import dependencies

## Training Process
- Obtain data from [open source](https://universe.roboflow.com/) . This example is using URL to download data in form of images and labels<br/>
- Check and change directory for training
- Train the YOLOv5s algorith with `data.yaml` and weights <br/>
**Note** You can use pretrained weights for any YOLOv5 architecture or just use `weights = ""` for randomized initial weights


## Testing the model
Just deploy using the `detect.py` provided in YOLOv5 repo <br/>
Remember to provide:
1. source (the images or video you want to test with)
2. data (the `data.yaml` for the classes)
3. weights (the trained model weight, we use `best.pt` in this example)
