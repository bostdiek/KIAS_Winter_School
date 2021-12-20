# KIAS Winter School - Intro to Machine Learning

## Technical Details
To use the tutorials, you will either need to have a python environment already setup with the packages from the `requirements.txt`, along with Tensorflow. If you do not have access to these, my environment, including python and jupyter notebooks can be downloaded using [Docker](https://www.docker.com/products/docker-desktop). Please have either a working environment or Docker already installed before the school. If using docker, please also run the following code before the first tutorial to download and install all of the packages. We will use the same call from the terminal each time we want to open the notebooks, but it will only download and install the first time.

Run the notebooks using:
```
docker run -p 8888:8888 -it -v $PWD:$PWD -w $PWD -e JUPYTER_ENABLE_LAB=yes bostdiek/kias_ws
```

To quit the notebooks, select `File > Shutdown` or hit `Control + C` in the terminal window.

To download the turorials, use
```git clone https://github.com/bostdiek/KIAS_Winter_School.git```.
Then move into that directory and launch the notebooks: `docker run -p 8888:8888 -it -v $PWD:$PWD -w $PWD -e JUPYTER_ENABLE_LAB=yes bostdiek/kias_ws`
