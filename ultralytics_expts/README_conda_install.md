As of 2024-04-09<br>
https://github.com/pytorch/vision#installation<br>
The following is the corresponding torchvision versions and supported Python versions.<br>
| torch | torchvision | Python |
| --- | --- | --- |
| main / nightly | main / nightly | >=3.8, <=3.11 |
| 2.2 | 0.17 | >=3.8, <=3.11 |
| 2.1 | 0.16 | >=3.8, <=3.11 |
| 2.0 | 0.15 | >=3.8, <=3.11 |

- conda create --name ultralytics-env python=3.8 -y
- conda activate ultralytics-env
- conda install -c conda-forge ultralytics-env
- conda install pytorch::pytorch
  - NOTE: pytorch is 2.2
- conda install torchvision=0.17
  - NOTE: doing **conda install torchvision** gave me version 0.15, did not work

$ yolo detect predict model=yolov8n.pt source='https://ultralytics.com/images/bus.jpg'<br>
- Ultralytics YOLOv8.1.45 Python-3.8.19 torch-2.2.2 CPU (Intel Core(TM) i7-6700K 4.00GHz)
- YOLOv8n summary (fused): 168 layers, 3151904 parameters, 0 gradients
- Found https://ultralytics.com/images/bus.jpg locally at bus.jpg
- image 1/1 D:\github-Mark-MDO47\MDOpythonUtils\ultralytics\bus.jpg: 640x480 4 persons, 1 bus, 1 stop sign, 123.0ms
- Speed: 3.0ms preprocess, 123.0ms inference, 1458.0ms postprocess per image at shape (1, 3, 640, 480)
- Results saved to runs\detect\predict2
- Learn more at https://docs.ultralytics.com/modes/predict
