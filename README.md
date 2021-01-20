# Anti-Candid_Pose
Anti-Candid_Pose

## 1. Enter Virtual Environment
source /home/minggatsby/python/bin/activate

## 2. Load Path
cd src/Anti-Candid/

## 3. Mode
### Object Detection

#### If it use gstreamer
python3 trt_yolo.py -m yolov4-416 --usb 0

#### If it doesn't use gstreamer
python3 trt_yolo.py -m yolov4-416 --usb 0 -g 


### Pose_Estimation

cd src/Anti-Candid/trt_pose/tasks/human_pose/

python3 detect_camera.py


### Object Detection & Pose_Estimation

#### If it use gstreamer
python3 main.py --usb 0

#### If it doesn't use gstreamer
python3 main.py --usb 0 -g 
