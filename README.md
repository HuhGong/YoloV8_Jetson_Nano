# YoloV8_Jetson_Nano


https://github.com/jetsonmom/yolov8_jetson4GB?tab=readme-ov-file


# make env


uname -a


wget https://github.com/Archiconda/build-tools/releases/download/0.2.3/Archiconda3-0.2.3-Linux-aarch64.sh
sudo chmod 755 Archiconda3-0.2.3-Linux-aarch64.sh


 ./Archiconda3-0.2.3-Linux-aarch64.sh 


 conda env list


 conda activate base

 
jetson_release 


conda create -n yolo python=3.8 -y


conda env list


conda activate yolo


 pip install -U pip wheel gdown


gdown https://drive.google.com/uc?id=1hs9HM0XJ2LPFghcn7ZMOs5qu5HexPXwM


gdown https://drive.google.com/uc?id=1m0d8ruUY8RvCP9eVjZw4Nc8LAwM8yuGV


sudo apt-get install libopenblas-base libopenmpi-dev


sudo apt-get install libomp-dev


pip install torch-1.11.0a0+gitbc2c6ed-cp38-cp38-linux_aarch64.whl


pip install torchvision-0.12.0a0+9b5a3fe-cp38-cp38-linux_aarch64.whl


python -c "import torch; print(torch.__version__)"

(yolo) dli@dli:~$ python


>>> import torch
>>> import torchvision
>>> print(torch.__version__)
>>> print(torchvision.__version__)
>>> print("cuda used", torch.cuda.is_available())

git clone https://github.com/Tory-Hwang/Jetson-Nano2


(yolo) dli@dli:~$ cd Jetson-Nano2/


(yolo) dli@dli:~/Jetson-Nano2$ cd V8


(yolo) dli@dli:~/Jetson-Nano2/V8$ pip install ultralytics


(yolo) dli@dli:~/Jetson-Nano2/V8$ pip install -r requirements.txt 


(yolo) dli@jdli:~/Jetson-Nano2/V8$ pip install ffmpeg-python


(yolo) dli@dli:~/Jetson-Nano2$ sudo apt install tree


(yolo) dli@jdli:~/Jetson-Nano2$ tree -L 2

gedit  detectY8.py

# in file "detectY8"


# change "brtsp: False"

(yolo) yolo@yolo-desktop:~/Jetson-Nano2/V8$ python detectY8.py

# if error code "import cv2" import cv2

# if error code "no module 'tensorboard'" pip install tensorboard






