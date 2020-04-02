# docker-pyqt5_02-04-2020
docker-pyqt5


Dockerfile for development of GUI applications with Python 3 + PyQt5

Tested on Ubuntu 16.04, 16.10, 18.10

https://github.com/jozo/docker-pyqt5

https://hub.docker.com/r/fadawar/docker-pyqt5/

How to use it
You can clone this github repository and then run this command to check if it's working

Run

docker run -it \
    -v /tmp/.X11-unix:/tmp/.X11-unix \
    -v $(pwd)/test:/app \
    -e DISPLAY=$DISPLAY \
    -u qtuser \
    fadawar/docker-pyqt5 python3 /app/hello.py
You should see window similar to this:

Screenshot

Build

docker build -t fadawar/pyqt5 .
Other Dockerfiles
Python 3 + PyQt5: https://github.com/jozo/docker-pyqt5

Python 3 + PyQt5 + QML: https://github.com/jozo/docker-pyqt5-qml

Python 3 + PyQt5 + QML + QtMultimedia: https://github.com/jozo/docker-pyqt5-qml-qtmultimedia
