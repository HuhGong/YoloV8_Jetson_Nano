# YoloV8_Jetson_Nano


How to use YoloV8 in Jetson nano


# i refer this site
# https://i7y.org/en/yolov8-on-jetson-nano/



# open terminal

sudo apt update


# install python 3.8


sudo apt install -y python3.8 python3.8-venv python3.8-dev python3-pip \
libopenmpi-dev libomp-dev libopenblas-dev libblas-dev libeigen3-dev libcublas-dev


![p1](https://github.com/user-attachments/assets/23df0d78-94ad-4638-b40e-651d180ad54a)

git clone https://github.com/ultralytics/ultralytics





![p2](https://github.com/user-attachments/assets/f55d3dca-3125-4d82-bc8f-5eb0b17234f3)


cd ultralytics



![p3](https://github.com/user-attachments/assets/5c7f943c-f89d-4a10-bc52-fad769dc88ac)

python3.8 -m venv venv


source venv/bin/activate


pip install -U pip wheel gdown



![p4](https://github.com/user-attachments/assets/bfc839f1-7fcc-4666-861e-a15ad200c280)


# pytorch 1.11.0


gdown https://drive.google.com/uc?id=1hs9HM0XJ2LPFghcn7ZMOs5qu5HexPXwM


# torchvision 0.12.0


gdown https://drive.google.com/uc?id=1m0d8ruUY8RvCP9eVjZw4Nc8LAwM8yuGV


python3.8 -m pip install torch-*.whl torchvision-*.whl


pip install .




![p5](https://github.com/user-attachments/assets/5a1952b5-3617-4fa1-a8e0-14724b878275)


yolo task=detect mode=predict model=yolov8n.pt source=0 show=True


yolo task=segment mode=predict model=yolov8n-seg.pt source=0 show=True

# if you want to stop camera press "esc"

![p6](https://github.com/user-attachments/assets/0abc136c-d8cd-48ed-92c8-35c920adb1f0)





![p7](https://github.com/user-attachments/assets/6a76f3bb-cee0-4255-a0f6-cf2f45ca8abf)


# If you want to put your video into yolo v8, just put the file into ultralytics.


yolo task=detect mode=predict model=yolov8n.pt source="goose/mov" show=True


yolo task=segment mode=predict model=yolov8n-seg.pt source="goose/mov" show=True


![p8](https://github.com/user-attachments/assets/f4baf021-d62b-4f43-9f56-c4172651f732)



https://github.com/user-attachments/assets/01f8961b-7b85-4883-92a6-3605f2ac54d3




