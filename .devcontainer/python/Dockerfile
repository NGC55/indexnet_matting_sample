# FROM python:3.9
FROM pytorch/pytorch:latest

WORKDIR /tmp/work

COPY requirements.txt ${PWD}

#RUN pip3 install numpy torch pandas matplotlib opencv-python
RUN apt-get update && apt-get upgrade -y

# OpenCV
RUN apt-get install -y libgl1-mesa-glx libglib2.0-0 libsm6 libxrender1 libxext6
RUN pip install opencv-python opencv-contrib-python

RUN pip install -r requirements.txt
