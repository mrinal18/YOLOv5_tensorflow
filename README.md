# Yolo5V

## Tensorflow

1. Install tensorflow, such as "sudo pip install tensorflow>=1.15 or tensorflow > 2.0" etc.

## Introduction
A tensorflow implementation of YOLOv5 inspired by [https://github.com/ultralytics/yolov5](https://github.com/ultralytics/yolov5).

Neck: SPP[[3]](https://arxiv.org/abs/1406.4729), PAN[[4]](https://arxiv.org/abs/1803.01534); 

Head: YOLOv5/YOLOv4(Mish), YOLOv3(Leaky_ReLU)[[10]](https://arxiv.org/abs/1804.02767); 

Loss: DIOU CIOU[[5]](https://arxiv.org/pdf/1911.08287v1.pdf), Focal_Loss[[6]](https://arxiv.org/abs/1708.02002);  Other: Label_Smoothing[[7]](https://arxiv.org/pdf/1906.02629.pdf);

## Environment

Python 3.6.8

Tensorflow 1.13.1 or Tensorflow 2.0 up

## Quick Start

1. Download YOLOv5 weights from [yolov5.weights](https://drive.google.com/open?id=1Drs_Aiu7xx6S-ix95f9kNsA6ueKRpN2J).

2. Train Yolov5.
3. Run Yolov5.

### Train

In core/config.py add your own path.

usage: python train.py gpu_id net_type(yolov5)

```
python train.py 0 yolov5
```

### Usage

Inference

```
python test.py
```

```
python demo.py
```

## Reference

[[1] Cross Stage Partial Network (CSPNet)](https://arxiv.org/pdf/1911.11929.pdf)

[[2] A Self Regularized Non-Monotonic Neural Activation Function](https://arxiv.org/abs/1908.08681)

[[3] Spatial Pyramid Pooling in Deep Convolutional Networks for Visual Recognition](https://arxiv.org/abs/1406.4729)

[[4] Path Aggregation Network for Instance Segmentation](https://arxiv.org/abs/1803.01534)

[[5] Distance-IoU Loss: Faster and Better Learning for Bounding Box Regression](https://arxiv.org/pdf/1911.08287v1.pdf)

[[6] Focal Loss for Dense Object Detection](https://arxiv.org/abs/1708.02002)

[[7] When Does Label Smoothing Help?](https://arxiv.org/pdf/1906.02629.pdf)

[[8] Convolutional Block Attention Module](https://arxiv.org/abs/1807.06521)

[[9] YOLOv4: Optimal Speed and Accuracy of Object Detection](https://arxiv.org/abs/2004.10934)

[[10] YOLOv3: An Incremental Improvement](https://arxiv.org/abs/1804.02767)

[[11] Aggregated Residual Transformations for Deep Neural Networks](https://arxiv.org/abs/1611.05431)

### Acknowledgment

keras_yolov3 [https://github.com/qqwweee/keras-yolo3](https://github.com/qqwweee/keras-yolo3).

keras_yolov4 [https://github.com/Ma-Dan/keras-yolo4](https://github.com/Ma-Dan/keras-yolo4).

