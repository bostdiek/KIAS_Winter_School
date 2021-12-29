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

## Repository Structure
```
├── Dockerfile
├── LICENSE
├── README.md
├── data
│   ├── top_tagging
│   │   ├── raw
│   │   │   ├── test.h5
│   │   │   ├── train.h5
│   │   │   └── val.h5
│   │   └── smaller_raw
│   │       ├── nsubjettiness_test.npy
│   │       ├── nsubjettiness_training.npy
│   │       ├── nsubjettiness_val.npy
│   │       ├── test_events.npy
│   │       ├── test_images.npy
│   │       ├── test_labels.npy
│   │       ├── training_events.npy
│   │       ├── training_images.npy
│   │       ├── training_labels.npy
│   │       ├── val_events.npy
│   │       ├── val_images.npy
│   │       └── val_labels.npy
│   ├── tutorial_1_data
│   │   ├── linear_regression_curved_test.npy
│   │   ├── linear_regression_curved_training.npy
│   │   ├── linear_testing.npy
│   │   ├── linear_training.npy
│   │   ├── logistic_regression_testing.npy
│   │   ├── logistic_regression_training.npy
│   │   └── logistic_regression_validation.npy
│   └── tutorial_2_data
│       ├── gluons.csv
│       └── quarks.csv
├── requirements.txt
├── slides
│   ├── KIAS_Ostdiek_MachineLearning_1.key
│   ├── KIAS_Ostdiek_MachineLearning_1.pdf
│   ├── KIAS_Ostdiek_MachineLearning_2.key
│   ├── KIAS_Ostdiek_MachineLearning_2.pdf
│   ├── KIAS_Ostdiek_MachineLearning_3.key
│   └── KIAS_Ostdiek_MachineLearning_3.pdf
└── tutorials
    ├── Tutorial1.ipynb
    ├── Tutorial1_Answers.ipynb
    ├── Tutorial2.ipynb
    ├── Tutorial2_Answers.ipynb
    ├── Tutorial3_0_TopTagging_ProcessRawData.ipynb
    └── Tutorial3_1_TopTagging_Visualizations.ipynb
```
