# KIAS Winter School - Intro to Machine Learning

## Technical Details
Run the notebooks using:
```
docker run -p 8888:8888 -it -v $PWD:$PWD -w $PWD -e JUPYTER_ENABLE_LAB=yes bostdiek/kias_ws
```

```
docker build --rm -t bostdiek/kias_ws:0.02 -t bostdiek/kias_ws .
```
