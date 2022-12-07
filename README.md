# YOLOv5 를 이용한 객체인식  
> 개발 환경
- 운영체제: Window10
- 가상환경: WSL2, Docker
- 컨테이너 내 운영체제: Ubuntu:20.04
> PC정보  

|하드웨어명|정보|
|---|:---|
|CPU|Intel(R) Core(TM) i7-8086K @ 4.00GHz(12CPUs)|
|GPU|NVIDIA Geforce RTX 2080 (16GB)|
|RAM|32GB|  

> 사용한 패키지

|패키지명|버전|
|---|:---|
|Python|3.9.6|
|Jupyter_client|7.4.7|
|CUDA|11.6|
|Pytorch|1.13|
|Pandas|1.5.2|
|Yolo|v5|
|OpenCV|4.6.0.66|
|Pillow|9.0.1|  

---  
> 데이터 정제  
- json파일에서 annotation 과 img_path 의 정보들을 추출
- 이미지 파일명과 레이블의 파일명을 anno_id로 통일화
- 레이블의 x,y,w,h 값들을 이미지 크기의 비율에서 정규화

> 모델 설명  
- 사용한 Yolo모델 : yolov5x
- Pre-trained 모델 : yolov5x
- 배치사이즈: 4
- 이미지 크기: 640
- 데이터 갯수: 4000
- epoch: 100
- Optimizer: SGD
- learning_rate: 0.01


> 학습결과

