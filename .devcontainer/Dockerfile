FROM python:latest

RUN apt-get update && apt-get install ffmpeg libsm6 libxext6  -y

# dev container necessities
RUN python3 -m pip install -U pylint

# other important packages
RUN python3 -m pip install -U packaging
RUN python3 -m pip install -U requests

# the machine learning dependencies
RUN python3 -m pip install -U numpy
RUN python3 -m pip install -U Pillow
RUN python3 -m pip install -U matplotlib
RUN python3 -m pip install -U opencv-python
RUN python3 -m pip install -U pandas
RUN python3 -m pip install -U scipy
RUN python3 -m pip install -U scikit-learn

RUN useradd -ms /bin/bash vscode

USER vscode
WORKDIR /home/vscode
