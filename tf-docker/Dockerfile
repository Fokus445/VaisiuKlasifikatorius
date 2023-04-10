FROM tensorflow/tensorflow:latest-gpu-jupyter

RUN apt-get update && apt-get install -y --no-install-recommends \
         libsm6 \
         libxext6 \
         libxrender-dev \
         ffmpeg && \
     rm -rf /var/lib/apt/lists/*

RUN pip install --upgrade pip
RUN pip install --upgrade wheel setuptools


RUN apt-get update && apt-get install -y --no-install-recommends \
        libaspell-dev


RUN pip install bs4 tensor2tensor aspell-python-py3


WORKDIR /tf