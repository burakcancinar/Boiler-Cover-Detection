# Boiler-Cover-Detection
<div align="left">
  <p>
    <a align="left" href="http://egerobot.com.tr" target="_blank">
      <img width="850" src="egerobot_logo_01.png"></a>
  </p>

  English | [简体中文](.github/README_cn.md)
  <br>
  <div>
    <a href="https://github.com/ultralytics/yolov5/actions/workflows/ci-testing.yml"><img src="https://github.com/ultralytics/yolov5/actions/workflows/ci-testing.yml/badge.svg" alt="YOLOv5 CI"></a>
    <a href="https://zenodo.org/badge/latestdoi/264818686"><img src="https://zenodo.org/badge/264818686.svg" alt="YOLOv5 Citation"></a>
    <a href="https://hub.docker.com/r/ultralytics/yolov5"><img src="https://img.shields.io/docker/pulls/ultralytics/yolov5?logo=docker" alt="Docker Pulls"></a>
    <br>
    <a href="https://bit.ly/yolov5-paperspace-notebook"><img src="https://assets.paperspace.io/img/gradient-badge.svg" alt="Run on Gradient"></a>
    <a href="https://colab.research.google.com/github/ultralytics/yolov5/blob/master/tutorial.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
    <a href="https://www.kaggle.com/ultralytics/yolov5"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>
  </div>

## <div align="left">Chemical Boiler Cover Detection</div>
>This project uses yolov5 and custom dataset to detect open cover boiler and closed cover boiler. I made a custom dataset for this project
>Some images for training data

![](screen2.jpg)



## <div align="left">Code</div>

```python3
!git clone https://github.com/ultralytics/yolov5  # clone repo
!pip install -U -r yolov5/requirements.txt  # install dependencies
```
>Custom Dataset
```python3
!python /content/yolov5/train.py --img 640 --batch 16 --epochs 200 --data /content/tank-7/data.yaml --weights yolov5x.pt
```
```python3
%cd /content/yolov5
```
>Test
```python3
!python /content/drive/MyDrive/yolov5/detect.py --weights /content/drive/MyDrive/egerobot1/best.pt --line-thickness 1 --img 640 --conf 0.40 --source /content/drive/MyDrive/egerobot/egerobotik3.mp4

```


## <div align="center">Youtube Video</div>
<a href="https://youtu.be/QixSkY5JUoE
" target="_blank"><img src="https://raw.githubusercontent.com/burakcancinar/Boiler-Cover-Detection/main/screen2.jpg" 
alt="Video" width="1280" height="600" border="10" /></a>
